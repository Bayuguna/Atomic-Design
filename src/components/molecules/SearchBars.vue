<template>
  <div>
    <b-input-group inline>
      <FormInput :size="size" placeholder="Search" />
      <ButtonIcon
        :size="size"
        :variant="variant"
        id="btn-search"
        :icon="icon"
      ></ButtonIcon>
    </b-input-group>
  </div>
</template>

<script>
import FormInput from "@/components/atoms/forms/FormInput.vue";
import ButtonIcon from "@/components/atoms/buttons/ButtonIcon.vue";
export default {
  name: "SearchBars",
  components: {
    FormInput,
    ButtonIcon,
  },
  data:()=>{
    return{
      size:'md',
      variant: 'success',
      icon: ['fas', 'search']
    }
  }
};
</script>

<style>

#btn-search .btn {
  border-radius: 0rem 0.25rem 0.25rem 0rem !important;
}
</style>