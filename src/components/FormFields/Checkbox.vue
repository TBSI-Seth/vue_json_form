<template>
  <b-checkbox :id="schemaName" ref="child" v-model="fieldData" :required="required" :name="title" :switch="switches"
              class="vjf_checkbox">
    <span v-if="ui.label || ui.label === undefined">{{ title }}</span>
  </b-checkbox>
</template>

<script>
import formFieldMixin from "./formFieldMixin.js";

//@group FormFields
/**
 * This is used to render booleans in Form of a checkbox
 */
export default {
  name: "Checkbox",
  mixins: [formFieldMixin],
}
</script>

<style scoped>

</style>
