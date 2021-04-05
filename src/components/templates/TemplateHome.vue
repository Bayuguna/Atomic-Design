<template>
  <div>
    <Navbar/>
    <ContentHome :settings="settings" :images="images"/>
  </div>
</template>

<script>
import ContentHome from "@/components/organisms/ContentHome.vue";
import Navbar from "@/components/organisms/Navbars.vue";

export default {
  name: "TemplateHome",
  props:{
    settings: Array,
    images: Array
  },
  components: {
    ContentHome,
    Navbar
  },
};
</script>

<style>
</style>