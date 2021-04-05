<template>
    <b-button v-if="block == true" :variant="variant" block>{{ title }}</b-button>
    <b-button v-else :variant="variant">{{ title }}</b-button>
</template>

<script>
export default {
  name: "Buttons",
  props: {
    variant: String,
    title: String,
    block: Boolean,
    type: String,
    icon: Array
  },
};
</script>

<style>
</style>