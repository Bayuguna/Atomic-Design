<template>
  <b-form-group label="Individual radios" v-slot="{ ariaDescribedby }">
    <b-form-radio
      v-for="(row, index) in radio"
      :key="index"
      :aria-describedby="ariaDescribedby"
      :name="name"
      :value="row.value"
      >{{ row.title }}</b-form-radio
    >
  </b-form-group>
</template>

<script>
export default {
    name: 'FormRadio',
    props:{
        radio: Array, // radio:[{value: '', title: ''}]
        name: String
    }
};
</script>

<style>
</style>