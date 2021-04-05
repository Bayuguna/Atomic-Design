<template>
  <b-form-file
    v-if="plain == true"
    :placeholder="placeholder"
    :accept="accept"
    drop-placeholder="Drop file here..."
  ></b-form-file>
</template>

<script>
export default {
    name: 'FormFile',
    props: {
        plain: Boolean,
        accept: String, //.jpg, .png, .gif
        placeholder: String
    }
};
</script>

<style>
</style>