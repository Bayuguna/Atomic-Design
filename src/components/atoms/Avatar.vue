<template>
  <b-avatar :variant="variant" :text="text" :src="src" :icon="icon"></b-avatar>
</template>

<script>
export default {
    name: 'Avatar',
    props: {
        variant: String,
        text: String,
        src: String,
        icon: String
    }
}
</script>

<style>

</style>