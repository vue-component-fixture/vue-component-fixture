<template>
  <input
    :id="'attribute-' + attribute"
    v-model="textValue"
    class="form-control"
  />
</template>
<script>
import { editorMixin } from "./EditorMixin";

export default {
  name: "string-attribute-editor",

  props: {
    value: {
      required: false,
      type: String
    }
  },

  mixins: [editorMixin],

  computed: {
    textValue: {
      get() {
        return this.value;
      },
      set(value) {
        this.updateIfValid(value);
      }
    }
  }
};
</script>
