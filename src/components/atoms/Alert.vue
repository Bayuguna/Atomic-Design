<template>
  <b-alert :variant="variant" show>{{title}}</b-alert>
</template>

<script>
export default {
    name: 'Alert',
    props:{
        variant: String,
        title: String
    }
}
</script>

<style>

</style>