<template>
  <b-form-radio-group
      :id="schemaName"
      v-model="fieldData"
      :options="options"
      :stacked="this.ui.options && this.ui.options.stacked"
      :required="required"
      :buttons="!!(this.ui.options && this.ui.options.buttons)"
      :button-variant="variant"
      class="vjf_radiobuttons"
  ></b-form-radio-group>
</template>

<script>
import formFieldMixin from "./formFieldMixin.js";

//@group FormFields
/**
 * This is used to render Radiobutton Groups (Selection of enum)
 */
export default {
  name: "Radiobuttons",
  mixins: [formFieldMixin],
  computed: {
    options() {
      function getTextForItem(options, key) {
        if (options?.enumTitles) {
          return options.enumTitles[key] || key;
        }
        return key;
      }
      let result = []
      if (this.item.enum){
        result = this.item.enum.map(key => {
          return {value: key, text: getTextForItem(this.ui.options, key)}
        })
      }
      return result
    }
  }
}
</script>

<style scoped>

</style>
