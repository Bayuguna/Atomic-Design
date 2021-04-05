<template>
  <div>
    <b-navbar-nav>
      <NavItem :to="route_beranda" :title="beranda" />
      <NavItem :to="route_umkm" :title="umkm" />
      <NavItem :to="route_shop" :title="shop" />
      <NavItem :to="route_page" :title="page" />
      <NavItem :to="route_contact" :title="contact" />
    </b-navbar-nav>
  </div>
</template>

<script>
import NavItem from "@/components/atoms/NavItem.vue";
export default {
  name: "NavbarMenus",
  components: {
    NavItem,
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
    };
  },
};
</script>

<style>
</style>