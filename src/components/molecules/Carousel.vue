<template>
  <VueSlickCarousel
    v-bind="settings"
  >
    <Images
    v-for="(row, index) in images" :key="index"
      :src="row.src"
    />
  </VueSlickCarousel>
</template>

<script>
import Images from "@/components/atoms/Images.vue";
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";
export default {
  name: "Carousel.vue",
  components: {
    Images,
    VueSlickCarousel,
  },
  props:{
      images: Array,
      arrow: Boolean,
      dots: Boolean,
      infinite: Boolean,
      autoplay: Boolean,
      settings: Array
  }
};
</script>

<style>
</style>