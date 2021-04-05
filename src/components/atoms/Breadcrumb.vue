<template>
  <b-breadcrumb :items="items"></b-breadcrumb>
</template>

<script>
export default {
    name: 'Breadcrumb',
    props:{
        items: Array //items: [{text: '', href: '' / to: {name: ''}, active: Boolean}]
    }
}
</script>

<style>

</style>