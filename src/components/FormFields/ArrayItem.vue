<template>
  <div class="vjf_arrayItem">
    <FormField ref="child" :json="json" :name="schemaName+index" :ui="ui" :array="index"
               @changedData="loopUp" noText :filledData="filledData">
      <b-button variant="outline-danger" @click="$emit('deleteItem', index)">
        <b-icon-x/>
      </b-button>
      <template v-slot:prepend>
        <b-button class="handle" disabled variant="outline-secondary">
          <b-icon-grip-vertical></b-icon-grip-vertical>
        </b-button>
      </template>
    </FormField>
    <hr v-if="divider">
  </div>
</template>

<script>
import formFieldMixin from "./formFieldMixin.js";

//@group FormFields
/**
 * This is used to render items in an array
 */
export default {
  name: "ArrayItem",
  mixins: [formFieldMixin],
  components: {FormField: () => import("./FormField.vue")},
  props: {
    //index in array
    index: {
      type: Number,
      required: true
    },
    //Is this item supposed to have a divider (`<hr>`) at the end?
    divider: {
      type: Boolean
    }
  },
  mounted() {
    this.$refs.child?.focus();
  },
  setChild(value) {
    console.log(value)
  }
}
</script>

<style scoped>

</style>
