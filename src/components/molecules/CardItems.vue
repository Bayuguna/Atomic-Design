<template>
  <div class="card" style="width: 18rem">
    <Images class="card-img-top" id="item-image" :src="src" alt="Card image cap" />
    <div class="card-body">
      <h5 class="card-title">{{title}}</h5>
      <p class="card-text">
        {{text}}
      </p>
      <Button :title="Dashboard" :block="true"></Button>
    </div>
  </div>
</template>

<script>
import Images from '@/components/atoms/Images.vue'
import Button from '@/components/atoms/buttons/Button.vue'
export default {
    name: 'CardItems',
    components:{
        Images,
        Button
    },
    props:{
        src: String,
        title: String,
        text: String,
        btn_title: String
    }
};
</script>

<style >

/* #item-image{
    width: 5rem !important;
} */
</style>