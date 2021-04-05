<template>
  <div>
    <b-row>
      <!-- <Icon icons="faw fa-person" /> -->
      <router-link to="/#"><Icon class="icon" :icon="icon1"/></router-link>
      <router-link to="/#"><Icon class="icon" :icon="icon2"/></router-link>
    </b-row>
  </div>
</template>

<script>
import Icon from '@/components/atoms/Icon.vue'
export default {
  name: "NavbarMenuRights",
  components: {
    Icon
  },
  data:()=>{
    return{
      icon1:['far', 'heart'],
      icon2:['fas', 'shopping-cart']
    }
  }
};
</script>

<style scoped>
.icon {
  margin: 10px;
  color: black;
}

</style>