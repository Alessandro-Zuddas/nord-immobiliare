<script>
export default {

    name: "MainTop",

    data() {
        return {
        
        }
    }
}
</script>

<template>

    <div class="container">
        <div class="row main-top-head">
            <h2 class="main-title">Specialisti delle costruzioni</h2>
            <hr>
            <p class="desc-text">
                In campo residenziale il design, la tecnologia all’avanguardia e la cura dei dettagli sono gli elementi che distinguono i nostri interventi.
                Per noi è fondamentale il rispetto per l’ambiente e l’utilizzo di materiali che ci consentono di superare i più rigorosi standard di sicurezza.
                Per questo motivo, da sempre, le nostre opere sono progettate per essere in armonia col paesaggio circostante.
            </p>
        </div>

        <!-- Company benefits -->
        <div class="row row-bt-circle justify-content-md-center justify-content-sm-center px-3">
            <!-- Company benefit One -->
            <div class="col-lg-2 col-md-10 col-sm-8 mx-lg-4">
                <i class="fa-regular fa-building card-icon"></i>
                <h3 class="card-title">Costruire</h3>
                <p class="card-text">
                    Il nostro lavoro ci piace, è la nostra grande passione. Vi garantiamo la qualità dei materiali, la competenza nei lavori e buoni prezzi per fornirvi il miglior servizio, avvalendoci dell'esperienza maturata con 30 anni di attività nel settore.
                </p>
            </div>
            <!-- /Company benefit One -->
            <!-- Company benefit two -->
            <div class="col-lg-2 col-md-10 col-sm-8">
                <i class="fa-solid fa-arrows-rotate card-icon"></i>
                <h3 class="card-title">Rinnovare</h3>
                <p class="card-text">
                    Siamo specialisti nello studio, nella progettazione e nella realizzazione di interventi di ristrutturazione per privati e per commerciali.
                </p>
            </div>
            <!-- /Company benefit two -->
            <!-- Company benefit three -->
            <div class="col-lg-2 col-md-10 col-sm-8 mx-lg-4">
                <i class="fa-sharp fa-solid fa-house card-icon"></i>
                <h3 class="card-title">Unicità</h3>
                <p class="card-text">
                    Quando costruiamo o ristrutturiamo, ai nostri clienti proponiamo sempre soluzioni sostenibili con l'ambiente e all'avanguardia nel campo del risparmio energetico.
                </p>
            </div>
            <!-- /Company benefit three -->
            <!-- Company benefit four -->
            <div class="col-lg-2 col-md-10 col-sm-8">
                <i class="fa-solid fa-truck card-icon"></i>
                <h3 class="card-title">Esclusività</h3>
                <p class="card-text">
                    Un Team di professionisti esperti e qualificati progetta assieme a voi, realizzando la soluzione più giusta per le vostre esigenze.
                </p>
            </div>
            <!-- /Company benefit four -->
        </div>
    </div>
    <!-- /Company benefits -->
    
    <!-- Company Infos -->
    <div class="row bg-variant d-none d-lg-flex d-md-flex d-sm-flex">   
        <div class="container-fluid">
            <!-- Company Info One -->
            <div class="company-infos">
                <i class="fa-solid fa-suitcase info-icon"></i>
                <h2 class="info-number">250+</h2>
                <p class="info-text">LAVORI ESEGUITI</p>
            </div>
            <!-- /Company Info One -->
            <!-- Company Info Two -->
            <div class="company-infos">
                <i class="fa-solid fa-building info-icon"></i>
                <h2 class="info-number">750+</h2>
                <p class="info-text">PROGETTI CREATI</p>
            </div>
            <!-- /Company Info Two -->
            <!-- Company Info Three -->
            <div class="company-infos">
                <i class="fa-solid fa-users info-icon"></i>
                <h2 class="info-number">20</h2>
                <p class="info-text">PROFESSIONISTI ESPERTI</p>
            </div>
            <!-- /Company Info Three -->
            <!-- Company Info Four -->
            <div class="company-infos">
                <i class="fa-sharp fa-solid fa-globe info-icon"></i>
                <h2 class="info-number">10+</h2>
                <p class="info-text">LAVORI INTERNAZIONALI</p>
            </div>
            <!-- /Company Info Four -->
        </div>
    </div>
    <!-- /Company Infos -->

</template>

<style lang="scss" scoped>

/* Company benefits */

.container{
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 4.6875rem 0;
}

.main-top-head{
    display: flex;
    flex-direction: column;
    align-items: center;
}

.main-title{
    color: var(--titles-color);
    padding-bottom: .625rem;
}

hr{
    width: 8%;
    height: .125rem;
    background-color: #fed03d;
    border: none;
}

.desc-text{
    font-size: 1.1875rem;
    text-align: center;
    margin-top: 1.5625rem;
    margin-bottom: 3.75rem;
}

.row{
    display: flex;
    justify-content: space-between;
    text-align: center;
    width: 100%;
    padding: 0 3.125rem;
}


.col-md-10{
    background-color: #f5f5f5;
    padding: 1.25rem .625rem;
    border-radius: .625rem;
    margin-bottom: 1.25rem;
}

.card-icon{
    display: flex;
    justify-content: center;
    align-items: center;
    margin: auto;
    width: 3.75rem;
    border-radius: 50%;
    aspect-ratio: 1;
    border: .0313rem solid var(--titles-color);
    color: var(--titles-color);
    font-size: 1.5625rem;
}

.card-title{
    color: var(--titles-color);
    font-size: 1.75rem;
}

.card-text{
    font-size: 1.125rem;
    margin-top: .625rem;
}

.card-icon,.card-title{
    font-weight: bold;
    margin-bottom: .625rem;
}

/* /Company benefits */

/* Company infos */

.row{
    margin: 0 0;
    padding: 0 0;
}

.bg-variant{
    padding: 1.5625rem 0;
    position: relative;
    overflow: hidden;
    background-image: url("../../../assets/img/home-244125289.jpg");
    background-size: cover;
    background-repeat: no-repeat;
}

.bg-variant:before{
    content: "";
    position: absolute;
    top: -30%;
    width: 100%;
    height: 50%;
    background-color: white;
    border-bottom-left-radius: 45%;
    border-bottom-right-radius: 45%; 
}

.bg-variant:after{
    content: "";
    position: absolute;
    width: 100%;
    bottom: -30%;
    height: 50%;
    background-color: white;
    border-top-left-radius: 45%;
    border-top-right-radius: 45%;
}

.container-fluid{
    display: flex;
    padding: 6.25rem 0;
}

.company-infos{
    width: calc(100% / 4);
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 3.125rem 0;
    color: var(--first-color);
}

.company-infos:hover{
    transform: scale(1.1);
}

.info-text{
    color: white;
    font-size: .875rem;
}

.info-icon{
    font-size: 3.125rem;
    margin-bottom: .3125rem;
}

.info-number{
    font-size: 2.5rem;
}

/* /Company infos */

</style>