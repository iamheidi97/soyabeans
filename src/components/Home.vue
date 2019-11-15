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
          <p class="text1 all-text">Be Japan-ready<br>in a month!</p>
          <img class="img-fluid" src="../assets/images/pham.jpg" alt="image slot" />
        </template>
      </b-carousel-slide>

      <!-- <b-carousel-slide>
        <template v-slot:img>
          <p class="text2 all-text">Immerse yourself with the<br><span class="emp-t2">Japanese Culture</span></p>
          <img class="img-fluid"   src="../assets/images/1.png" alt="image slot" />
        </template>
      </b-carousel-slide> -->
      <b-carousel-slide>
        <template v-slot:img>
          <p class="text2 all-text">Immerse yourself with the<br><span class="emp-t2">Japanese Culture</span></p>
          <img class="img-fluid"   src="../assets/images/2.png" alt="image slot" />
        </template>
      </b-carousel-slide>

      <b-carousel-slide>
        <template v-slot:img>
          <p class="text3 all-text text-right mr-5">Receive expert advise on<span class="emp-t3"><br>Great Travel Locations<br></span>for your trip</p>
          <img class="img-fluid" src="../assets/images/castle5.jpg" alt="image slot" />
        </template>
      </b-carousel-slide>

    </b-carousel>
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
.emp-t3{
  color: #fffb25;
  background-color: transparent;
  /* text-shadow: 4px 4px 0px #2c3e50; */
  text-shadow: 3px 3px 0px #b4b4b4;
  /* color: #2c3e50; */
  font-size: 3.8rem;
}
.emp-t2{
  color: rgb(255, 72, 47);
  background-color: transparent;
  /* text-shadow: 4px 4px 0px #2c3e50; */
  text-shadow: 3.8px 3.8px 0px rgb(255, 255, 214);
  /* color: #2c3e50; */
  font-size: 4rem;
}
p.text3{
  transform: translate(-5%, -50%);
  top: 40%;
  font-size: 3.4rem;
}
p.text2{
  font-size: 3.4rem;
  transform: translate(50%, -52%);
  top: 52%;
  right: 50%;
  background-color: transparent;
  line-height: 100%;
  color: rgb(0, 119, 255);
  text-shadow: 3px 3px 0px rgb(255, 255, 255);
}
p.text1 {
  text-align: left;
  transform: translate(75%, -55%);
  top: 40%;
  right: 20%;
  font-size: 4rem;
}
.all-text{
  /* right: 35%; */
  position: absolute;
  background-color: transparent;
  font-weight: bold;
  color: #fff9ba;
  width: 100%;
  text-shadow: 4px 4px 0px #4f9e37;
}
.my-home {
  overflow: hidden;
  box-sizing: border-box;
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
  .all-text { 
    font-size: 2.6em;  
  }
  .emp-t2, .emp-t3{
    font-size: 2.8em;
  }
}
@media (max-width: 768px) {
  .all-text {
    font-size: 2.5rem;
  }
  .emp-t2, .emp-t3{
    font-size: 2.6rem;
  }
}
@media (max-width: 668px) {
  .all-text {
    font-size: 2rem;
  }
  .emp-t2, .emp-t3{
    font-size: 2.1rem;
  }
}
@media (max-width: 530px) {
  .all-text {
    font-size: 1.5rem;
  }
  .emp-t2, .emp-t3{
    font-size: 1.6rem;
  }
}
@media (max-width: 360px) {
  .all-text{
    font-size: 1rem;
  }
  .emp-t2, .emp-t3{
    font-size: 1rem;
  }
}

</style>
