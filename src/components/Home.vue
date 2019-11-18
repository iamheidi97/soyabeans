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
          <p class="all-text text1">
            Be Japan-ready
            <br />in a month!
          </p>
          <img class="img-fluid" src="../assets/images/pham.jpg" alt="image slot" />
        </template>
      </b-carousel-slide>

      <b-carousel-slide>
        <template v-slot:img>
          <p class="all-text text2 ">
            Immerse yourself with the
            <br />
            <span class="emp-t2">Japanese Culture</span>
          </p>
          <img class="img-fluid" src="../assets/images/2.png" alt="image slot" />
        </template>
      </b-carousel-slide>

      <b-carousel-slide>
        <template v-slot:img>
          <p class="all-text text3 text-right mr-5">
            Receive expert advise on
            <span class="emp-t3">
              <br />Great Travel Locations
              <br />
            </span>for your trip
          </p>
          <img class="img-fluid" src="../assets/images/castle5.jpg" alt="image slot" />
        </template>
      </b-carousel-slide>

      <b-carousel-slide>
        <template v-slot:img>
          <p class="all-text text4 text-left">
            Prices start at <br><span class="price">Php 500</span> for <br> one-on-one<br> classes
          </p>
          <img class="img-fluid" src="../assets/images/shibuya.jpg" alt="image slot" />
        </template>
      </b-carousel-slide>

      <b-carousel-slide>
        <template v-slot:img>
          <p class="all-text text5 text-right">
            Make the most<br>of your journey
            <br />
            <span class="emp-t5">Learn Japanese</span><br>as you travel Cebu
          </p>
          <img class="img-fluid" src="../assets/images/cebu.jpg" alt="image slot" />
        </template>
      </b-carousel-slide>

    </b-carousel>
    <img src="../assets/whiteskewed.svg" class="img-fluid w-100 upperslight" />

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
/* .flip-horizontal {
  -webkit-transform: scaleX(-1);
  transform: scaleX(-1);
} */
.upperslight {
  position: relative;
  margin-top: -8%;
  z-index: 1000;
}
.skewed {
  transform: skewY(5deg);
  transform-origin: top right;
}

.all-text {
  position: absolute;
  background-color: transparent;
  font-weight: bold;
  color: #fff9ba;
  width: 100%;
  text-shadow: 4px 4px 0px #4f9e37;
}

/* cebu */
.emp-t5 {
  color: #fffb25;
  background-color: transparent;
  text-shadow: 3px 3px 0px #b4b4b4;
}
p.text5 {
  transform: translate(-2%, -60%);
  top: 40%;
  font-size: 3.7em;
  line-height: 120%;
}

/* shibuya */
.emp-t4 {
  color: #fffb25;
  background-color: transparent;
  text-shadow: 3px 3px 0px #b4b4b4;
  font-size: 1.5em;
}
p.text4 {
  transform: translate(45%, -20%);
  top: 20%;
  left: 45%;
  font-size: 3.4em;
  width: 40%;
  line-height: 100%;
  color: #23A262;
  text-shadow: 3px 3px 0px #fff9ba;
}


.price {
  color: rgb(255, 78, 78);
  text-shadow: 3px 3px 0px #fff9ba;
  font-style: italic;
}

/* castle */
.emp-t3 {
  color: #fffb25;
  background-color: transparent;
  text-shadow: 3px 3px 0px #b4b4b4;
}
p.text3 {
  transform: translate(-5%, -50%);
  top: 40%;
  font-size: 2.8em;
  line-height: 120%;
}

/* anime */
.emp-t2 {
  color: rgb(255, 72, 47);
  background-color: transparent;
  text-shadow: 3px 3px 0px rgb(255, 255, 214);
}
p.text2 {
  line-height: 100%;
  color: rgb(18, 120, 253);
  text-shadow: 3px 3px 0px rgb(255, 255, 244);
  transform: translate(5%, 60%);
  top: 40%;
  font-size:3.2rem!important;
}

/* main */
p.text1 {
  text-align: left;
  transform: translate(75%, -55%);
  top: 40%;
  right: 20%;
  font-size: 3.4em;
  line-height: 120%;
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

@media (max-width: 1060px) {
  p.text1{
    font-size: 3em;
  }
  /* p.text2{

  }
  p.text3{

  } */
  p.text4{
    font-size: 2.6em;
  }
  p.text5{
    font-size: 1.8em;
  }
}

@media (max-width: 930px) {
  p.text1{
    font-size: 2.6em;
  }
  p.text3{
    font-size: 2rem;
  }
  p.text4{
    font-size: 2rem;
  }
  p.text5{
    font-size: 1.5rem;
  }
  p.text2 {
    font-size: 1.6rem !important;
    top:36%;
  }
}

@media (max-width: 767.5px) {
  p.text1{
    font-size: 2rem;
  }
  p.text2{
    font-size: 2rem !important;
    top:36%;
  }
  /* p.text3{

  }
  p.text4{
    
  } */
  p.text5 {
    font-size: 2em;
  }
}

@media (max-width: 768px) {
  p.text1{
    text-shadow: 2px 2px 0px #4f9e37;
    font-size:2rem!important;
  }
  p.text2{
    font-size:1.5rem!important;
    text-shadow: 1px 1px 0px rgb(255, 255, 244);
  }
  .emp-t2 {
    text-shadow: 1px 1px 0px rgb(255, 255, 214);
  }
  p.text3{
    font-size:1.5rem!important;
  }
  .emp-t3 {
    font-size:1.5rem!important;
  }
  p.text4{
    text-shadow: 2px 2px 0px #fff9ba;
    left: 40%;
    top:25%;
  }
  .price {
    text-shadow: 1px 1px 0px #23A262;
  }
  p.text5 {
    font-size:1.5rem!important;
  }
  .emp-t5 {
    text-shadow: 1px 1px 0px #b4b4b4 !important;
  }
  .emp-t4,
  .emp-t3,
  .emp-t4 {
    text-shadow: 1px 1px 0px #b4b4b4;
  }

  .all-text {
    text-shadow: 1px 1px 0px #4f9e37;
  }
  
}
@media (max-width: 575.5px) {
  p.text1{
    font-size: 1rem!important;
  }
  p.text2{
    font-size: 1rem !important;
    text-shadow: 1px 1px 0px rgb(255, 255, 244);
  }
  .emp-t2 {
    text-shadow: 1px 1px 0px rgb(255, 255, 214);
  }
  p.text3{
    font-size: 1rem !important;
  }
  .emp-t3 {
    font-size: 1rem !important;
  }
  p.text4{
    font-size: 1rem;
  }
  .price {
    text-shadow: 1px 1px 0px #23A262;
  }
  p.text5 {
    font-size: 1rem !important;
  }
  .emp-t5 {
    text-shadow: 1px 1px 0px #b4b4b4 !important;
  }
}

</style>
