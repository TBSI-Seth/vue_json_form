<template>
  <FormField :class="'vjf_control '+hiddenClass+customCss" @changedData="loopUp" :json="json" :ui="ui" :name="ui.scope"
             :filled-data="filledData">
    <span v-if="ui.options && ui.options.append">{{ ui.options.append }}</span>
  </FormField>
</template>

<script>
import layout from "./layoutMixin.js";
import FormField from "../FormFields/FormField.vue";

//@group Layouts
export default {
  name: "Control",
  components: {FormField},
  mixins: [layout],
  computed: {
    hiddenClass() {
      return this.ui.options?.hidden?'hiddenControl':''
    },
  }
}
</script>

<style scoped>
.hiddenControl {
  display: none;
}
</style>
