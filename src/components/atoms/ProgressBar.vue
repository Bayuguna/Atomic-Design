<template>
    <b-progress class="mt-2" :max="max" show-value>
      <b-progress-bar v-for="(row, index) in progress" :key="index" :value="row.value" :variant="row.variant"></b-progress-bar>
    </b-progress>
</template>

<script>
export default {
    name: 'ProgressBar',
    props: {
        max: Number,
        variant: String,
        progress: Array //progress: [{value: int, variant: ''}]
    }
}
</script>

<style>

</style>