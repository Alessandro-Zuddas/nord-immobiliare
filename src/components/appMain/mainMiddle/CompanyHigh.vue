<script>

export default {

  name: "CompanyHigh",

  data() {
      return {
      
    }
  }
}
</script>

<template>
  
  <!-- Componente highligths -->
  <div class="container-fluid bg-variant">
    <!-- Main Middle Two Header -->
    <div class="container-sm sm-three">
      <h2 class="main-title">Valori chiave</h2>
      <hr>
      <p class="desc-text">
        La Nord Immobiliare nasce ad Olbia, nei primi anni del 2000. Oggi come allora, sotto la guida del GEOM. Egidio Zuddas, è operativa nel settore immobiliare di tutto il Nord-Sardegna per quanto riguarda la costruzione di complessi residenziali, residenze private e lavori di ristrutturazione di qualsiasi genere.
      </p>
      <!-- /Main Middle Two Header -->

      <!-- Company Highligts -->
      <div class="row">
        <!-- High One -->
        <div class="col-lg-3 col-md-6 col-sm-6 d-flex flex-column align-items-center text-center">
          <div class="highligts high-one">
            <i class="fa-sharp fa-solid fa-house high-icon"></i>
          </div>
          <strong class="high-title">
            Qualità
          </strong>
          <hr class="high-line">
          <p class="high-text">
            Ottieni le soluzioni intelligenti e di alta qualità, perfette a livello funzionale, in grado di durare nel tempo e capaci di farti vivere meglio.
          </p>
        </div>
        <!-- /High One -->
        <!-- High Two -->
        <div class="col-lg-3 col-md-6 col-sm-6 d-flex flex-column align-items-center text-center">
          <div class="highligts high-two">
            <i class="fa-solid fa-gear  high-icon"></i>
          </div>
          <strong class="high-title">
            Sicurezza:
          </strong>
          <hr class="high-line">
          <p class="high-text">
            Vivi la serenità di vedere realizzati i tuoi progetti a norma di legge, secondo le direttive attuali e nel completo rispetto della sicurezza dei cantieri.
          </p>
        </div>
        <!-- /High Two -->
        <!-- High Three -->
        <div class="col-lg-3 col-md-6 col-sm-6 d-flex flex-column align-items-center text-center">
          <div class="highligts high-three">
            <i class="fa-solid fa-users high-icon icon-three"></i>
          </div>
          <strong class="high-title">
            Affidabilità:
          </strong>
          <hr class="high-line">
          <p class="high-text">
            Fidati del nostro geometra e dei seri artigiani che da oltre 30 anni svolgono il loro lavoro con perizia, passione e assoluta affidabilità.
          </p>
        </div>
        <!-- /High Three -->
        <!-- High Four -->
        <div class="col-lg-3 col-md-6 col-sm-6 d-flex flex-column align-items-center text-center">
          <div class="highligts high-four">
            <i class="fa-solid fa-lightbulb high-icon"></i>
          </div>
          <strong class="high-title">
            Semplicità:
          </strong>
          <hr class="high-line">
          <p class="high-text">
            Evita lo stress di organizzare muratori, elettricisti, imbianchini, etc. Dal progetto alla messa in opera, da noi avrai solo un unico referente.
          </p>
        </div>
        <!-- /High Four -->
      </div>
      <!-- /Company Highligts -->
    </div>
  </div>
  <!-- Componente highligths -->

</template>

<style lang="scss" scoped>

.container-fluid{
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-top: 3.125rem;
}

.main-title{
  color: var(--titles-color);
  padding-bottom: .625rem;
  padding-top: 2.1875rem;
}

hr{
  width: 6.25rem;
  height: .125rem;
  background-color: #fed03d;
  border: none;
}

.desc-text{
  font-size: 1.1875rem;
  text-align: center;
  margin-top: 1.5625rem;
  margin-bottom: 2.5rem;
}

.container-sm{
  display: flex;
  justify-content: center;
  padding-bottom: 3.125rem;
}

.row{
  display: flex;
  justify-content: space-between;
  width: 100%;
}

.container-fluid{
  padding: 0;
}

.sm-three{
  display: flex;
  flex-direction: column;
  align-items: center;
}


.highligts{
  display: flex;
  justify-content: center;
  align-items: center;
  border: none;
  border-radius: 50%;
  aspect-ratio: 1;
}

.highligts:hover{
  background-color: var(--first-color);
}

.high-one{
  background-color: #4ea4a5;
}

.high-two{
  background-color: #3f7ff7;
}

.high-three{
  background-color: #f6722a;
}

.high-four{
  background-color: #a7cf47;
}

.high-icon{
  color: white;
  font-size: 2.1875rem;
  padding: 2.1875rem 2.1875rem;
}

.icon-three{
  font-size: 28px;
}

.high-title{
  color: var(--titles-color);
  margin-top: .625rem;
  margin-bottom: .625rem;
}

.high-line{
  width: 20%;
}

.high-text{
  color: var(--titles-color);
  font-size: 1rem;
  margin-top: .9375rem;
}

</style>