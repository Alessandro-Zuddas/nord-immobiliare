<script>
export default {

    name: "AppGallery",

    data() {
        return {

          galleryImages: [

            {
              imgSrc: "https://via.placeholder.com/400",
              imgAlt: "Image One",
              isVisible: true,
            },
            {
              imgSrc: "https://via.placeholder.com/400",
              imgAlt: "Image One",
              isVisible: true,
            },
            {
              imgSrc: "https://via.placeholder.com/400",
              imgAlt: "Image One",
              isVisible: true,
            },
            {
              imgSrc: "https://via.placeholder.com/400",
              imgAlt: "Image One",
              isVisible: true,
            },
            {
              imgSrc: "https://via.placeholder.com/400",
              imgAlt: "Image One",
              isVisible: false,
            },
            {
              imgSrc: "https://via.placeholder.com/400",
              imgAlt: "Image One",
              isVisible: false,
            },
            {
              imgSrc: "https://via.placeholder.com/400",
              imgAlt: "Image One",
              isVisible: false,
            },
            {
              imgSrc: "https://via.placeholder.com/400",
              imgAlt: "Image One",
              isVisible: false,
            },

          ]

        }
    }
}
</script>

<template>
  
    <!-- Componente galleria -->
    <!-- Main Middle One Header -->
    <h2 class="main-title">I nostri lavori</h2>
    <hr>
    <p class="desc-text">
      La galleria dei lavori da noi realizzati è in costante aggiornamento per consentire una visione generale del nostro operato <br> e per permettere a chiunque di trovare ispirazione attraverso esso. 
    </p>
    <!-- /Main Middle One Header -->

    <!-- Projects Images -->
    <div class="container-sm">
      <div class="row">
        <div v-for="img in this.galleryImages" v-show="img.isVisible === true"
        class="col-12 col-sm-6 col-md-6 col-lg-6 col-xl-3 gy-3">
          <img class="project-img" :src="img.imgSrc" alt="Project One Image">
        </div>
      </div>
    </div>
    <!-- /Projects Images -->

    <div class="container-sm sm-two">
      <div class="column">
        <hr class="all-projects-line">
      </div>
      <div class="column">
        <h5 class="all-projects-text">
          <a class="all-pj-link" href="#">VIEW ALL PROJECTS</a>
        </h5>
      </div>
      <div class="column">
        <hr class="all-projects-line"> 
      </div>
    </div>
    <!-- Componente galleria -->

</template>

<style lang="scss" scoped>


/* Projects Images */

.main-title{
  color: var(--titles-color);
  padding-bottom: .625rem;
  padding-top: .9375rem;
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
}

.project-img{
  max-width: 100%;
  border-radius: .625rem;
}

.column:hover{
  .hover-panel{
    display: flex;
  }
}

.row{
  display: flex;
  justify-content: space-between;
  width: 100%;
}

.col-12{
  text-align: center;
}

.column{
  position: relative;
  width: calc(100% / 3);
  text-align: center;
}

.sm-two{
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 1.25rem;
  margin-bottom: 2.5rem;
}

.all-projects-text{
  padding: 1.25rem 0;
  padding-bottom: .625rem;
}

.all-pj-link{
  text-decoration: none;
  color: var(--first-color);
}

.all-pj-link:hover{
  color: var(--titles-color);
}

.all-projects-line{
  width: 100%;
  background-color: lightgray;
}

/* /Projects Images */

</style>