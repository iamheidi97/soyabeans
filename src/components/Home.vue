<template>
     <div>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Text slides with image -->

      <b-carousel-slide>
        <template v-slot:img>
          <img
            class="d-block img-fluid w-100"
            width="1024"
            height="480"
            src="../assets/images/castle2.jpg"
            alt="image slot"
          >
        </template>
      </b-carousel-slide>

      <!-- <b-carousel-slide>
        <template v-slot:img>
          <img
            class="d-block img-fluid w-100"
            width="1024"
            height="480"
            src="../assets/images/calligraphy.jpg"
            alt="image slot"
          >
        </template>
      </b-carousel-slide> -->

      <b-carousel-slide>
        <template v-slot:img>
          <img
            class="d-block img-fluid w-100"
            width="1024"
            height="480"
            src="../assets/images/anime.jpg"
            alt="image slot"
          >
        </template>
      </b-carousel-slide>

    </b-carousel>

    <p class="mt-4 d-none">
      Slide #: {{ slide }}<br>
      Sliding: {{ sliding }}
    </p>
  </div>
</template>
<script>
      export default {
    data () {
      return {
        publicPath: process.env.BASE_URL,
        slide: 0,
        sliding: null,
      }
    },
    methods: {
      // eslint-disable-next-line no-unused-vars
      onSlideStart (slide) {
        this.sliding = true
      },
      // eslint-disable-next-line no-unused-vars
      onSlideEnd (slide) {
        this.sliding = false
      }
    }
  }
</script>
<style scoped>
.my-home{
  background-position: center; 
  overflow: hidden;
  box-sizing: border-box;
  height: 100vh;
}
.carousel-item{
  overflow: hidden;
  box-sizing: border-box;
  min-height: 100%;
  max-height: 100%;
  max-width: 100%;
}
</style>
