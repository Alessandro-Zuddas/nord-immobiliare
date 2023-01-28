<script>
export default {

    name: "HeroBottom",

    data() {
        return {
        
        }
    }
}
</script>

<template>
  <!-- Hero Bottom -->
  <div class="container-fluid cont-two d-none d-lg-block d-md-block">
    <div class="container-sm">
      <div class="row">
        <!-- Hero Left -->
        <div class="col-lg-6 col-md-12 mb-md-5 d-lg-flex d-md-flex flex-column align-items-center justify-content-center text-center d-none">
          <h2 class="hero-title-two">Costruiamo i tuoi sogni</h2>
          <hr class="hero-bt-line">
          <p class="hero-two-text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus magnam, distinctio itaque architecto cupiditate consequuntur labore, minus quos quasi saepe adipisci vitae error.
          </p>
        </div>
        <!-- /Hero Left -->
        <!-- Hero right -->
        <div class="col-lg-6 col-md-12 mt-md-5 d-lg-flex d-md-flex flex-column align-items-center d-none">
          <button class="hero-btn">GET A FREE QUOTE!</button>
          <small class="free-trial-text">Only takes a few seconds!</small>
        </div>
        <!-- /Hero right -->
      </div>
    </div>
  </div>
  <!-- /Hero Bottom -->
</template>

<style scoped>

/* Hero Bottom Down */

.cont-two{
  padding: 9.375rem 0;
  background-image: url(../../assets/img/about-call-to-action-57862405.jpg);
  background-position: bottom;
  background-size: cover;
}

.hero-title-two{
  color: white;
  padding-bottom: 1.25rem;
}

.hero-bt-line{
  width: 20%;
  height: .625rem;
  background-color: rgb(255, 225, 0);
  margin: .3125rem 0;
  margin-bottom: 1.5625rem;
}

.hero-two-text{
  color: white;
}

.hero-btn{
  color: var(--titles-color);
  background-color: var(--first-color);
  border: none;
  padding: .625rem 1.5625rem;
  margin-bottom: .3125rem;
  cursor: pointer;
}

.hero-btn:hover{
  color: white;
  background-color: var(--second-color);
}

.free-trial-text{
  color: white;
  font-size: .75rem;
}

</style>