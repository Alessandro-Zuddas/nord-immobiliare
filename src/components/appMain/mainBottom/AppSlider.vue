<script>
export default {

    name: "AppSlider",

    data() {
      return {
        carouselIndex: 0,
      }
    },
    methods:{
      onPrevClick(){

        if(this.carouselIndex === 0){
          
          this.carouselIndex++;

        }else{
          this.carouselIndex = 0;
        }

      },
      onNextClick(){

        if(this.carouselIndex === 1){
          
          this.carouselIndex--;

        }else{
          this.carouselIndex = 1;
        }

      }
    }
}
</script>

<template>

  <!-- Reviews -->
  <div class="container-fluid">
    <div class="row bg-variant">   
      <div class="container-sm sm-boots">
        <h2 class="main-bt-title">Our Home Owners Say</h2>
        <hr>
        <img v-show="(this.carouselIndex === 0)" class="review-img" src="../../../assets/img/home-testimonial-113165296.jpg" alt="Testimonial 1">
        <img v-show="(this.carouselIndex === 1)" class="review-img" src="../../../assets/img/home-testimonial-84268399.jpg" alt="Testimonial 2">
        <p v-show="(this.carouselIndex === 0)" class="review-text">
          "No man but feels more of a man in the world if he have but a bit of ground that he can call his own. However small it is on the surface, it is four thousand miles deep: and that is a very handsome property"
        </p>
        <p v-show="(this.carouselIndex === 1)" class="review-text">
          "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Voluptatem distinctio quod culpa perferendis quo quae ipsum id quas similique, numquam accusantium ipsa aliquid deserunt ad in pariatur."
        </p>
        <strong v-show="(this.carouselIndex === 0)" class="review-user">
          KATE HARRIS - NEW HOME OWNER
        </strong>
        <strong v-show="(this.carouselIndex === 1)" class="review-user">
          HARRY SMITH - NEW HOME OWNER
        </strong>
        <div class="carousel-index">
          <div class="car-dot" :class="{ active: carouselIndex === 0 }"></div>
          <div class="car-dot" :class="{ active: carouselIndex === 1 }"></div>
        </div>
        <!-- Carousel Buttons -->
        <button class="prev-btn" @click="onPrevClick">
          <i class="fa-solid fa-chevron-left prev-icon"></i>
        </button>
        <button class="next-btn" @click="onNextClick">
          <i class="fa-solid fa-chevron-right next-icon"></i>
        </button>
        <!-- /Carousel Buttons -->
      </div>
    </div>
  </div>
  <!-- /Reviews -->

</template>

<style lang="scss" scoped>

/* Reviews */

.container-fluid{
  margin: 0 0;
  padding: 0 0;
}

.sm-boots{
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 1.25rem 0;
}

.main-bt-title{
  color: white;
  padding-top: 9.375rem;
}

hr{
  width: 25%;
  margin: .9375rem 0;
  height: .125rem;
  background-color: #fed03d;
  border: none;
}

.review-text{
  color: rgba(255, 255, 255, 0.9);
  font-style: italic;
  text-align: center;
  margin-bottom: 1.5625rem;
}

.review-user{
  color: white;
}

.carousel-index{
  display: flex;
  color: white;
}

.car-dot{
  width: .625rem;
  height: .625rem;
  border-radius: 50%;
  border: 0.5px solid white;
  margin: 3.75rem .25rem;
}

.active{
  background-color: white;
}

.prev-btn, .next-btn{
  background: none;
  border: none;
}
.prev-btn{
  position: absolute;
  left: 5%;
}

.next-btn{
  position: absolute;
  right: 5%;
}

.prev-btn:hover,.next-btn:hover{
  transform: scale(1.2);
}

.prev-icon, .next-icon{
  font-size: 1.875rem;
  color: white;
}

.bg-variant{
  position: relative;
  overflow: hidden;
  background-image: url("../../../assets/img/home-parallax-144609983.jpg");
  background-repeat: no-repeat;
  background-position: left;
  background-size: cover;
}

.bg-variant:before{
  content: "";
  position: absolute;
  top: -30%;
  width: 100%;
  height: 50%;
  background-color: lightgray;
  border-bottom-left-radius: 45%;
  border-bottom-right-radius: 45%;
  background-color: #f5f5f5; 
}


.bg-variant{
  margin: 0;
  padding: 0;
}

.review-img{
  border-radius: 50%;
  aspect-ratio: 1;
  padding: .9375rem .9375rem;
  margin-bottom: 1.5625rem;
}

.container-sm{
  display: flex;
  padding: 6.25rem 0;
}

/* /Reviews */

</style>