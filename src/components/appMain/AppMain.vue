<script>

import MainTop from './mainTop/MainTop.vue';
import MainMiddle from './mainMiddle/MainMiddle.vue';
import MainBottom from './mainBottom/MainBottom.vue';

export default {

    name: "AppMain",

    components: {

      MainTop,
      MainMiddle,
      MainBottom,

    },
    data() {
      return {
      
      }
    }
}
</script>

<template>

  <MainTop />
  <MainMiddle />
  <MainBottom />

</template>

<style scoped>



</style>