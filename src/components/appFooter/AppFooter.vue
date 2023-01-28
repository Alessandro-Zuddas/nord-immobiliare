<script>
export default {

    name: "AppFooter",

    data() {
        return {
        
        }
    }
}
</script>

<template>

  <!-- Footer Top -->
  <div class="container-fluid">
    <div class="row justify-content-space-between">
      <!-- Footer Col One -->
      <div class="col-lg-3 col-md-3 col-sm-5 mt-4">
        <img src="../../assets/img/footer-logo.png" alt="">
        <p class="footer-text">
          
Siamo specialisti nella costruzione di immobili unici ed esclusivi. Il nostro lavoro ispira. Siamo orgogliosi di offrire qualità e design eccezionali per clienti in tutto il mondo.
        </p>
        <button class="learn-more-btn">SCOPRI DI PIU</button>
      </div>
      <!-- /Footer Col One -->
      <!-- Footer Col two -->
      <div class="col-lg-3 col-md-3 col-sm-5 mt-4">
        <strong class="col-title">CONTATTACI</strong>
        <div class="icon-plus-text">
          <i class="fa-sharp fa-solid fa-globe contact-us-icon"></i>
          <small class="col-three-text">
            Corporate Location <br>
            1600 Amphitheatre Parkway <br>
            London WC1 1BA
          </small>
        </div>
        <div class="icon-plus-text">
          <i class="fa-solid fa-house contact-us-icon"></i>
          <small class="col-three-text">
            Residential Location <br>
            9521 Broadsberry Avenue <br>
            Paddington RC7 9ZA
          </small>
        </div>
        <div class="icon-plus-text">
          <i class="fa-solid fa-phone-flip contact-us-icon-two"></i>
          <small class="col-three-text">1.800.458.556 / 1.800.532.2112</small>
        </div>
        <div class="icon-plus-text">
          <i class="fa-regular fa-envelope contact-us-icon-two"></i>
          <small class="col-three-text">info@your-domain.com</small>
        </div>
        <div class="icon-plus-text">
          <i class="fa-regular fa-clock contact-us-icon-two"></i>
          <small class="col-three-text">Monday - Friday: 9:00 AM - 6:00 PM</small>
        </div>
        <div class="icon-plus-text">
          <i class="fa-regular fa-clock contact-us-icon-two"></i>
          <small class="col-three-text">Saturday - Sunday: 9:00 AM - 12:00 PM</small>
        </div>
      </div>
      <!-- /Footer Col two -->
      <!-- Footer Col three -->
      <div class="col-lg-3 col-md-3 col-sm-12 d-flex flex-column mt-4">
        <strong class="col-title">DOVE TROVARCI</strong>
        <img class="find-us-img" src="../../assets/img/construction_map_pin.png" alt="">
      </div>
      <!-- /Footer Col three -->
    </div>
    <!-- /Footer Top -->

    <!-- Footer Bottom -->
    <div class="container-fluid cont-two">
      <div class="row ms-row align-items-center">
        <small class="footer-bt-text col-12 col-lg-5 col-md-5 text-center mt-3">
          COPYRIGHT 2023 SITE BY <strong>Alessandro Zuddas</strong> | ALL RIGHTS RESERVED | POWERED BY <strong>Nome Server</strong>
        </small>
        <div class="icons-container-bt col-12 col-lg-5 col-md-5 text-center text-lg-end mt-3">
          <a class="social-icons" href="#"><i class="fa-brands fa-facebook-f"></i></a>
          <a class="social-icons" href="#"><i class="fa-brands fa-twitter"></i></a>
          <a class="social-icons" href="#"><i class="fa-brands fa-youtube"></i></a>
          <a class="social-icons" href="#"><i class="fa-brands fa-instagram"></i></a>
        </div>
      </div>
    </div>
    <!-- Footer Bottom -->
  </div>

</template>

<style scoped>

/* Footer top */

.container-fluid{
  padding: 0;
}

.row{
  display: flex;
  justify-content: space-between;
  width: 100%;
  background-color: #1e1e1e;
  margin: 0;
  padding: 1.5625rem 1.5625rem;
  color: lightgray;
}

.footer-text{
  color: var(--titles-color);
  margin: 1.5625rem 0;
}

.learn-more-btn{
  color: var(--second-color);
  background-color: var(--first-color);
  border: none;
  padding: .5rem 1.25rem;
  cursor: pointer;
}

.learn-more-btn:hover{
  background-color: var(--second-color);
  color: white;
}

.col-title{
  color: var(--first-color);
  margin-bottom: 1.25rem;
}


.icon-plus-text{
  display: flex;
  color: var(--titles-color);
  margin-top: 1.25rem;
}

.contact-us-icon{
  padding-top: .625rem;
}

.contact-us-icon-two{
  padding-top: .375rem;
}


.col-three-text{
  margin-left: .625rem;
  margin-top: .3125rem;
}

.find-us-img{
  margin-top: .625rem;
  max-width: 18.75rem;
  max-height: 15.625rem;
}

/* /Footer top */

/* Footer bottom */

.cont-two{
  display: flex;
  justify-content: space-between;
  padding: 1.5625rem 2.5rem; 
  background-color: black; 
  color: var(--titles-color);
}

.ms-row{
  background-color: black;
}

.footer-bt-text{
  font-size: .75rem;
}

.icons-container-bt{
  margin-right: 3.125rem;
}

.social-icons{
  color: var(--titles-color);
  padding: 0 .3125rem;
}

/* /Footer bottom */

</style>