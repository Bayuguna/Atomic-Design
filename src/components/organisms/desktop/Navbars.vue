<template>
  <div>
    <b-container fluid="sm">
      <b-row id="navbar-head" align-v="center" class="mx-auto">
        <div class="col-lg-3 col-md-4 col-3">
          <Images id="logo-image" :src="logo" />
        </div>
        <div class="col-lg-6 col-md-4 col-9 col-centered">
          <SearchBar />
        </div>
        <div class="col-lg-3 col-md-4 col">
          <NavbarMenuRight class="float-right" />
        </div>
      </b-row>
    </b-container>
    <b-navbar toggleable="lg" type="dark">
      <!-- <b-navbar-brand href="#">{{ title }}</b-navbar-brand> -->
      <div class="container">
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <NavbarMenu />

          <!-- Right aligned nav items -->
        </b-collapse>
      </div>
    </b-navbar>
  </div>
</template>

<script>
// @ is an alias to /src
import NavbarMenu from "@/components/molecules/NavbarMenus.vue";
import NavbarMenuRight from "@/components/molecules/NavbarMenuRights.vue";
import Images from "@/components/atoms/Images.vue";
import SearchBar from "@/components/molecules/SearchBars.vue";

export default {
  name: "NavbarWeb",
  props: {
    title: String,
  },
  components: {
    NavbarMenu,
    NavbarMenuRight,
    Images,
    SearchBar,
  },

  data: () => {
    return {
      logo: "umkm_logo.png",
    };
  },
};
</script>

<style scoped>
#logo-image {
  width: 5rem;
}
#navbar-head {
  margin: 0.5rem;
}
#brand-image {
  width: 20%;
}

nav {
  background-color: rgb(2, 54, 2);
}
.navbar {
  padding: 0rem 0rem !important;
}
</style>