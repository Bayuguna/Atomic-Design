<template>
  <b-form-textarea
      :placeholder="placeholder"
      :size="size"
      :rows="rows"
      :max-rows="max_rows"
    ></b-form-textarea>
</template>

<script>
export default {
    name: 'FormTextarea',
    props:{
        placeholder: String,
        size: String,
        rows: String,
        max_rows: String
    }
}
</script>

<style>

</style>