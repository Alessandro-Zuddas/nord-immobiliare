<script>

import AppSlider from './AppSlider.vue';
import FormPrev from './FormPrev.vue';

export default {

    name: "MainBottom",

    components:{

      AppSlider,
      FormPrev,

    },
    data() {
      return {
        
      }
    },
    methods:{

    }
}
</script>

<template>

  <FormPrev />  

  <AppSlider /> 

</template>

<style lang="scss" scoped>


</style>