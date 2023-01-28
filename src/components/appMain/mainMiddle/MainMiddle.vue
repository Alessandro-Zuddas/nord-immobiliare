<script>

import AppGallery from './AppGallery.vue';
import CompanyHigh from './CompanyHigh.vue';

export default {

  name: "MainMiddle",

  components: {

    AppGallery,
    CompanyHigh,

  },

  data() {
      return {
      
    }
  }
}
</script>

<template>
  
  <div class="container-fluid">

    <AppGallery />

    <CompanyHigh />

  </div>

</template>

<style lang="scss" scoped>

.container-fluid{
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 0;
  padding-top: 3.125rem;
}

</style>