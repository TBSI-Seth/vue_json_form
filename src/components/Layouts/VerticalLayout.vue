<template>
  <div :class="'vjf_horizontal '+customCss">
    <form-wrap @changedData="loopUp" v-for="(item, index) in ui.elements" :ui="item" :json="json"
               :key="ui.toString().length+'_'+index" :filledData="filledData" :form-i-d="formID"></form-wrap>
  </div>
</template>

<script>
/* eslint-disable vue/no-unused-components */
import layoutMixin from "./layoutMixin.js";

//@group Layouts
/**
 * Layout, that displays its elements horizontally
 */
export default {
  name: "VerticalLayout",
  components: {
    FormWrap: () => import('../FormWrap.vue')
  },
  mixins: [layoutMixin]
}
</script>

<style scoped>

</style>
