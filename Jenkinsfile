pipeline {
  agent {
    dockerfile true

  }
  stages {
    stage('Preparation') {
      parallel {
        stage('Dependencies') {
          steps {
            sh 'npm ci'
          }
        }

        stage('Information') {
          steps {
            sh 'node -v'
            sh 'npm -v'
          }
        }

      }
    }
    stage('Test') {
        steps {
            sh 'sed -i.bak \'s/smokeTestTimeout: 10000/smokeTestTimeout: 60000/\' node_modules/cypress/lib/tasks/verify.js'
            sh 'node_modules/.bin/cypress install'
            sh 'npm run cy:verify'
            sh 'npm test'
        }
    }
    stage('Build') {
      parallel {
        stage('Build NPM') {
          steps {
            sh 'npm run build:npm'
            sh 'npm run zip:npm'
            archiveArtifacts 'dist.zip'
          }
        }

        stage('Build Demo') {
          steps {
            sh 'npm run build:demo'
            sh 'npm run zip:demo'
            archiveArtifacts 'demo.zip'
          }
        }

        stage('Lint') {
          steps {
            sh 'npm run lint'
          }
        }

      }
    }

  }

  post {
      always {
          archiveArtifacts 'cypress/videos/*'
          archiveArtifacts 'cypress/screenshots/*'
          junit 'test-results.xml'
      }
   }

  environment {
    HOME = '.'
  }
}
