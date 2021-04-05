<template>
    <b-sidebar :id="id" :title="title" shadow>
      <div class="px-3 py-2">
        <ul>
          <NavItem to="/" title="Beranda" />
          <NavItem to="/about" title="UMKM" />
          <NavItem to="/shop" title="Shop" />
          <NavItem to="/page" title="Page" />
          <NavItem to="/contact" title="Contact Us" />
        </ul>
      </div>
    </b-sidebar>
</template>

<script>
import NavItem from "@/components/atoms/NavItem.vue";
export default {
  name: "Sidebars",
  components: {
    NavItem,
  },
  props: {
    id: String,
    title: String,
  },
  data: () => {
    return {
      //title
      beranda: "Beranda",
      umkm: "UMKM",
      shop: "Shop",
      page: "Page",
      contact: "Contact Us",
      //route
      route_beranda: '/',
      route_umkm: '/umkm',
      route_shop: '/shop',
      route_page: '/page',
      route_contact: '/contact',
    }
  }
};
</script>

<style>
</style>