<template>
  <b-form-checkbox
      :value="value"
      :unchecked-value="unchecked_value"
    >
      {{title}}
    </b-form-checkbox>
</template>

<script>
export default {
    name: 'FormCheckbox',
    props: {
        value: String,
        unchecked_value: String,
        title: String
    }

}
</script>

<style>

</style>