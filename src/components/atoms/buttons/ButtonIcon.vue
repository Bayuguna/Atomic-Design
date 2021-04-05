<template>
  <div>
        <b-button :size="size" :variant="variant"><font-awesome-icon :icon="icon"/></b-button>
    </div>
</template>

<script>
export default {
    name: 'ButtonIcons',
    props: {
        icon: Array,
        variant: String,
        size: String
    }
}
</script>

<style>

</style>