<template>
  <input
    type="text"
    :value="modelValue"
    class="w-full text-lg font-normal focus:outline-none"
    @input="handleInput"
  />
</template>

<script>
export default {
  name: "TextInput",
  props: {
    modelValue: {
      type: String,
      required: true,
    },
  },
  emits: ["update:model-value"],
  methods: {
    handleInput($event) {
      this.$emit("update:model-value", $event.target.value);
    },
  },
};
</script>
