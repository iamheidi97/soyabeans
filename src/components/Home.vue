<template>
  <div>
    <!-- <Jumbotron/> -->
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="white"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Text slides with image -->

      <b-carousel-slide>
        <template v-slot:img>
          <p class="text1">Be Japan-ready in a month!</p>
          <img class="img-fluid" src="../assets/images/castle5.jpg" alt="image slot" />
        </template>
      </b-carousel-slide>

      <b-carousel-slide>
        <template v-slot:img>
          <img class="img-fluid" src="../assets/images/img5.jpg" alt="image slot" />
        </template>
      </b-carousel-slide>

      <b-carousel-slide>
        <template v-slot:img>
          <img class="img-fluid" src="../assets/images/a1.jpg" alt="image slot" />
        </template>
      </b-carousel-slide>

      <b-carousel-slide>
        <template v-slot:img>
          <img class="img-fluid" src="../assets/images/a2.jpg" alt="image slot" />
        </template>
      </b-carousel-slide>

      <b-carousel-slide>
        <template v-slot:img>
          <img class="img-fluid" src="../assets/images/a3.jpg" alt="image slot" />
        </template>
      </b-carousel-slide>

      <b-carousel-slide>
        <template v-slot:img>
          <img class="img-fluid" src="../assets/images/a4.jpg" alt="image slot" />
        </template>
      </b-carousel-slide>

      <b-carousel-slide>
        <template v-slot:img>
          <img class="img-fluid" src="../assets/images/a5.jpg" alt="image slot" />
        </template>
      </b-carousel-slide>

      <b-carousel-slide>
        <template v-slot:img>
          <img class="img-fluid" src="../assets/images/a6.jpg" alt="image slot" />
        </template>
      </b-carousel-slide>

      <b-carousel-slide>
        <template v-slot:img>
          <img class="img-fluid" src="../assets/images/a7.jpg" alt="image slot" />
        </template>
      </b-carousel-slide>

    </b-carousel>
    <!-- <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none">
      <polygon fill="white" points="0,0 0,20 100,20 100,10"/>
    </svg>-->
    <img src="../assets/skewedrectangle.svg" class="img-fluid w-100 upperslight" />

    <SoyaDescription />
    <p class="mt-4 d-none">
      Slide #: {{ slide }}
      <br />
      Sliding: {{ sliding }}
    </p>
  </div>
</template>
<script>
//  import Jumbotron from "./Jumbotron";
import SoyaDescription from "./SoyaDescription";
export default {
  components: {
    SoyaDescription
  },
  data() {
    return {
      publicPath: process.env.BASE_URL,
      slide: 0,
      sliding: null
    };
  },
  methods: {
    // eslint-disable-next-line no-unused-vars
    onSlideStart(slide) {
      this.sliding = true;
    },
    // eslint-disable-next-line no-unused-vars
    onSlideEnd(slide) {
      this.sliding = false;
    }
  }
};
</script>
<style scoped>
.upperslight {
  position: relative;
  margin-top: -10%;
  z-index: 1000;
}
.skewed {
  transform: skewY(5deg);
  transform-origin: top right;
}
.text1 {
  text-align: left;
  position: absolute;
  top: 40%;
  right: 25%;
  transform: translate(70%, -55%);
  color: #fff9ba;
  background-color: transparent;
  font-weight: bold;
  font-size: 3.5rem;
  width: 50%;
  padding-right: 3em;
  /* line-height: 95%; */
  /* text-shadow: px 1px 0px #4f9e37; */
  text-shadow: 4px 4px 0px #4f9e37;
}
.my-home {
  background-position: center;
  height: 100vh;
}
.carousel-item {
  overflow: hidden;
  box-sizing: border-box;
}
.skew {
  position: absolute;
  top: 0;
  bottom: 0;
  right: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: linear-gradient(#ff9d2f, #ff6126);
  transform: skewY(5deg);
  transform-origin: top right;
}

@media (max-width: 930px) {
  .text1 {
    font-size: 2.8rem;
  }
}
@media (max-width: 768px) {
  .text1 {
    font-size: 2.5rem;
  }
}
@media (max-width: 668px) {
  .text1 {
    font-size: 2rem;
  }
}
@media (max-width: 530px) {
  .text1 {
    font-size: 1.5rem;
  }
}
@media (max-width: 360px) {
  .text1 {
    font-size: 1rem;
  }
}
</style>
