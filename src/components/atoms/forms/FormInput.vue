<template>
        <b-form-input :size="size" :placeholder="placeholder"></b-form-input>
</template>

<script>
export default {
    name: 'TextInputs',
    props:{
        size: String,
        placeholder : String
    }
}
</script>

<style>

</style>    