<template>
  <div>
    <b-table striped :items="items"></b-table>
  </div>
</template>

<script>
export default {
    name: 'Table',
    props: {
        items: Array
    }
}
</script>

<style>

</style>