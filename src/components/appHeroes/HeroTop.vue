<script>
export default {

    name: "HeroTop",

    data() {
        return {
        
        }
    }
}
</script>

<template>
  
  <div class="container-fluid cont-one">
    <div class="img-container">
      <h1 class="hero-top-title">BUILDING INSPIRING SPACES</h1>
      <h4 class="hero-top-desc">Lascia che i tuoi sogni siano il nostro progetto</h4>
      <button class="hero-top-btn btn-one mt-2">ESPLORA I LAVORI RECENTI</button>
      <button class="hero-top-btn btn-two mt-2">RICHIEDI UN PREVENTIVO GRATUITO</button>
    </div>
  </div>

  <div class="container-fluid bg-variant">
    <h2 class="hero-top-title-two">Hai in mente un'idea che potremmo realizzare per te?</h2>
  </div>

</template>

<style scoped>

.container-fluid{
  text-align: center;
  background-image: url("../../assets//images/piscina2.jpg");
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
}

.cont-one{
  padding: 15.625rem 0;
}

.hero-top-title{
  font-size: 2.5rem;
  color: var(--second-color);
}

.bg-variant{
  position: relative;
  background-color: var(--first-color);
  padding: 3.125rem 0;
  background-image: none;
}

.hero-top-title-two{
  font-size: 1.5rem;
  font-weight: bold;
}

.hero-top-desc{
  color: var(--first-color);
  font-size: 1.5rem;
  margin: .9375rem 0;
}

.hero-top-btn{
  border: none;
  padding: .625rem .9375rem;
  cursor: pointer;
}

.btn-one{
  color: white;
  background-color: var(--second-color);
  margin-right: .625rem;
}

.btn-one:hover{
  color: var(--titles-color);
  background-color: var(--first-color);
}

.btn-two{
  background-color: var(--first-color);
  color: gray;
}

.btn-two:hover{
  background-color: var(--second-color);
  color: white;
}

</style>