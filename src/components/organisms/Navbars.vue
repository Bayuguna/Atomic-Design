<template>
  <div>
    <NavbarMobile id="navbar-mobile"/>
    <NavbarWeb id="navbar-web" />
  </div>
</template>

<script>
import NavbarMobile from "@/components/organisms/mobile/Navbars.vue";
import NavbarWeb from "@/components/organisms/desktop/Navbars.vue";
export default {
  name: "Navbar",
  components: {
    NavbarMobile,
    NavbarWeb,
  },
};
</script>

<style scoped>
@media (max-width: 992px) {
  nav {
    background-color: #ffffff;
  }
  .navbar {
    padding: 0rem 0rem !important;
  }

  .navbar-nav {
    padding: 0rem 0rem !important;
    text-align: center;
  }

  .nav-item a {
    color: black;
  }
  .navbar-toggler {
    background-color: #c0f052 !important;
  }

  #navbar-web {
    display: none;
  }
  #navbar-mobile {
    display: block !important;
  }
  
}

#navbar-mobile {
  display: none;
}
</style>