<template>
  <b-badge v-if="pill == true" pill :variant="variant">{{ title }}</b-badge>
  <b-badge v-else :variant="variant">{{ title }}</b-badge>
</template>

<script>
export default {
  name: "Badge",
  props: {
    variant: String,
    title: String,
    pill: Boolean,
  },
};
</script>

<style>
</style>