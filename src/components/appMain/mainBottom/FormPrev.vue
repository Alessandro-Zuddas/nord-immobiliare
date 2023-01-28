<script>
export default {

    name: "FormPrev",

    data() {
      return {
        
      }
    },
    methods:{

    }
}
</script>

<template>

  <!-- Sezione preventivi  -->
  <div class="container-fluid cont-two">
    <div class="container-sm ms-sm">
      <!-- Sezione preventivi  header -->
      <h2 class="main-title">Richiedi un preventivo gratuito!</h2>
      <hr class="latest-news-hr">
      <p class="desc-text text-center">
        Richiedi un preventivo in maniera completamente GRATUITA e in pochissimi click! <br> Un responsabile si occuperà di tutto e potresti realizzare al più presto la casa dei tuoi sogni!
      </p>
      <!-- /Sezione preventivi  header -->

      <div class="row g-2 form-preventivi">
        <!-- Form preventivi -->
        <form class="text-center" action="" method="get">
          <div class="col-md pb-2">
          <div class="form-floating">
            <input type="email" class="form-control" id="floatingInputGrid" placeholder="nome@esempio.it" value="nome@esempio.it" required>
            <label for="floatingInputGrid">Indirizzo Email</label>
          </div>
          </div>
          <div class="col-md pb-2">
            <div class="form-floating">
              <select class="form-select" id="floatingSelectGrid">
                <option selected>Scegli la tipologia</option>
                <option value="1">Nuova costruzione</option>
                <option value="2">Ristrutturazione</option>
                <option value="3">Altro</option>
              </select>
              <label for="floatingSelectGrid">Quale lavoro vorresti eseguire?</label>
            </div>
          </div>
          <div class="col-md pb-2">
            <div class="form-floating">
              <input type="tel" class="form-control" id="floatingInputGrid" placeholder="+39 3331234567" value="+39 333 1234567" required>
              <label for="floatingInputGrid">Numero di telefono</label>
            </div>
          </div>
          <button class="btn btn-primary mx-1 my-1" type="submit">Conferma</button>
          <button class="btn btn-secondary mx-1 my-1">Cancella</button>
          <strong class="form-text d-block">Un responsabile ti contatterà nel minor tempo possibile!</strong>
          <!-- /Form preventivi -->
        </form>
      </div>
    </div>
  </div>
  <!-- /Sezione preventivi -->

</template>

<style lang="scss" scoped>

.container-fluid{
  margin: 0 0;
  padding: 0 0;
  border-radius: .625rem;
}

.main-title{
  color: var(--titles-color);
}

.desc-text{
  font-size: 1.125rem;
}

.cont-two{
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: #f5f5f5;
}

.ms-sm{
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 0 0;
  margin-top: 3.125rem;
  margin-bottom: 3.125rem;
}

.row{
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;  
}

.form-preventivi{
  margin: 1.5625rem 0;
}

.form-text{
  text-align: center;
  padding: .3125rem 0;
}


/* Preventivi */

</style>