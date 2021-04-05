<template>
  <div class="shop">
    <Navbar/>
    <FormSelect :options="options"/>
    <FormCheckboxGroup name="fruits" id="fruit-1" :options="options"/>
    <FormRadio name="fruits" :radio="radio"/>
    <ProgressBar :max="max" :progress="progress"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/organisms/Navbars.vue'
import FormSelect from '@/components/atoms/forms/FormSelect.vue'
import FormRadio from '@/components/atoms/forms/FormRadio.vue'
import FormCheckboxGroup from '@/components/atoms/forms/FormCheckboxGroup.vue'
import ProgressBar from '@/components/atoms/ProgressBar.vue'

export default {
  name: 'Shop',
  components: { 
    Navbar,
    FormSelect,
    FormCheckboxGroup,
    FormRadio,
    ProgressBar
  },
  data() {
    return {
      max: 100,
      options: [{text: 'Apple', value:"Apple"},{text: 'Banana', value:"Banana"} ],
      radio: [{value:"Apple", title: "Apple"},{value:"Banana", title: "Banana"} ],
      progress: [{value: 20, variant: 'success'}, {value: 30}]
    }
  },
}
</script>
