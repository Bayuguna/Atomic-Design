<template>
  <b-list-group>
    <router-link v-for="(row, index) in lists" :key="index" :to="row.to"><b-list-group-item>{{row.title}}</b-list-group-item></router-link>
  </b-list-group>
</template>

<script>
export default {
    name: 'ListGroup',
    props:{
        lists: Array, // lists: [{to: '', title: ''}]
    }
};
</script>

<style>
</style>