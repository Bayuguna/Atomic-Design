<template>
  <div class="home">
   <TemplateHome :settings="settings" :images="images"/>
  </div>
</template>

<script>
// @ is an alias to /src
import TemplateHome from '@/components/templates/TemplateHome.vue'

export default {
  name: 'Home',
  components: {
    TemplateHome,
  },
  data() {
    return {
      images: [
        {
          src:
            "https://cdn.acodez.in/wp-content/uploads/2019/05/How-to-implement-animations-in-the-web-design.png",
        },
        {
          src:
            "https://cdn.acodez.in/wp-content/uploads/2019/05/How-to-implement-animations-in-the-web-design.png",
        },
        {
          src:
            "https://cdn.acodez.in/wp-content/uploads/2019/05/How-to-implement-animations-in-the-web-design.png",
        },
      ],
      settings: [
        {
          dots: true,
          dotsClass: "slick-dots custom-dot-class",
          edgeFriction: 0.35,
          infinite: false,
          speed: 500,
          slidesToShow: 1,
          autoPlay: true,
          slidesToScroll: 1,
        },
      ],
    };
  },
}
</script>
