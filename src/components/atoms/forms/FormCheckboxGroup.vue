<template>
    <b-form-group label="Using options array:" v-slot="{ ariaDescribedby }">
      <b-form-checkbox-group
        v-model="selected"
        :options="options"
        :aria-describedby="ariaDescribedby"
        :name="name"
      ></b-form-checkbox-group>
    </b-form-group>

</template>

<script>
export default {
  name: "FormCheckboxGroup",
  props: {
    options: Array, //options: [{text: '', value: '', disabled: Boolean}]
    name: String
  },
};
</script>

<style>
</style>