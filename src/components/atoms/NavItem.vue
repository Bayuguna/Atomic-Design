<template>
  <b-nav-item class="mr-4 nav-item">
    <router-link class="nav-link" :to="to">{{ title }}</router-link>
  </b-nav-item
  >
</template>

<script>
export default {
  name: "NavItem",
  props: {
    to: String,
    title: String,
  },
};
</script>

<style scoped>
@media (max-width: 992px) {
  .nav-item a {
    color: black !important;
    font-size: 0.9rem;
    padding: 0.8rem;
  }
}
.nav-item a {
  color: white;
  font-size: 0.8rem;
  padding: 0.5rem;
}
.nav-item a:hover {
  color: white;
  background-color: #28a745;
  text-decoration: none;
}
</style>