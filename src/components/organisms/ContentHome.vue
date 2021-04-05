<template>
  <div>
    <Carousel :images="images" :settings="settings" />
    <b-container>
      <b-row align-v="center">
        <b-col>
          <ListGroup :lists="lists"/>
        </b-col>
        <b-col>
           <CardItem src="umkm_logo.png" title="Hai" btn_title="Product" />
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import CardItem from "@/components/molecules/CardItems.vue";
import Carousel from "@/components/molecules/Carousel.vue";
import ListGroup from "@/components/atoms/ListGroup.vue";
export default {
  name: "CardItems",
  props:{
    images: Array,
    settings: Array
  },
  components: {
    CardItem,
    Carousel,
    ListGroup
  },
  data() {
    return {
      lists:[{to: '/', title: 'Pertanian'}, {to: '/', title: 'Perikanan'}, {to: '/', title: 'Perumahan'}]
    }
  },
};
</script>

<style>
</style>