<template>
  <b-form-select
      id="inline-form-custom-select-pref"
      class="mb-2 mr-sm-2 mb-sm-0"
      :options="options"
    ></b-form-select>
</template>

<script>
export default {
  name: 'FormSelect',
  props:{
    options: Array //options: [{text: '', value: ''}]
  }
}
</script>

<style>

</style>