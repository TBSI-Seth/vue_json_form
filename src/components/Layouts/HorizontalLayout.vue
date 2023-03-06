<template>
      <b-row :class="'vjf_horizontal '+customCss">
        <div :class="setColumnWidth(item)" v-for="(item, index) in ui.elements" :key="ui.toString().length+'_'+index">
          <form-wrap @changedData="loopUp" :json="json" :ui="item" :filledData="filledData"
                     :form-i-d="formID"></form-wrap>
        </div>
      </b-row>
</template>

<script>
import layout from "./layoutMixin.js";

//@group Layouts
/**
 * Layout, that displays its elements horizontally
 */
export default {
  name: "HorizonzalLayout",
  mixins: [layout],
  methods: {
    setColumnWidth(item){
      return item && item.options && item.options.columnWidth && parseInt(item.options.columnWidth) > 0 && parseInt(item.options.columnWidth) <= 12 ? 'col-' + item.options.columnWidth : 'col'
    }
  }
}
</script>

<style scoped>
.col {
  padding: 0;
}
</style>
