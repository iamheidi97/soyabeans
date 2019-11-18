<template>
  <div class="my-why">
    <h3 class="display-4 font-weight-bolder my-5 green-text justify-content-center">Why choose us?</h3>

    <div class="row justify-content-center my-5">
      <div class="col-lg-5 col-sm-9 col-6 align-self-center">
        <p class="mb-0 text-right why-bolder">Get fast results with our native Japanese sensei.</p>
        <p
          class="text-right"
        >Not only can we teach you the Japanese language, we can also help you learn more about the Japanese culture, places to go and must-try cuisines.</p>
      </div>
      <div class="col-lg-5 col-sm-3 col-3">
        <h1 class="display-1 text-center circle-behind font-weight-bolder text-light">1</h1>
      </div>
    </div>

    <div class="row justify-content-center my-5">
      <div class="col-lg-5 col-sm-3 col-3">
        <h1 class="display-1 text-center circle-behind font-weight-bolder ml-auto text-light">2</h1>
      </div>
      <div class="col-lg-5 col-sm-9 col-6 align-self-center">
        <p class="mb-0 text-left why-bolder">We have schedules and lessons tailored for you.</p>
        <p
          class="text-left"
        >Afraid of not being able to catch up fast enough? Busy? No worries, we can make sure that you can take your lessons at your own pace.</p>
      </div>
    </div>
    
    <div class="row justify-content-center my-5">
      <div class="col-lg-5 col-sm-9 col-6 align-self-center">
        <p class="mb-0 text-right why-bolder">Planning to take the JLPT later?</p>
        <p
          class="text-right"
        >Our lessons are formulated according to the JLPT standards. You can definitely use any of our courses later on as you expand your knowledge in Japanese.</p>
      </div>
      <div class="col-lg-5 col-sm-3 col-3">
        <h1 class="display-1 text-center circle-behind font-weight-bolder text-light">3</h1>
      </div>
    </div>

  </div>
</template>
<script>
</script>
<style scoped>
  @media (max-width: 576px) {
    .circle-behind {
        font-size: 3.5em;
      }
      .display-4 {
        font-size: 2.8rem;
      }
  }

  /* // Medium devices (tablets, 768px and up) */
  @media (min-width: 768px) {  }

  /* // Large devices (desktops, 992px and up) */
  @media (min-width: 992px) {  }

  /* // Extra large devices (large desktops, 1200px and up) */
  @media (min-width: 1200px) { }
.why-bolder {
  font-weight: 700;
  font-size: 1.2rem;
}
.circle-behind {
  background: #23a262;
  max-width: 8rem;
  min-width: 5rem;
  width:100%;
  height: auto;
  border-radius: 50%;
  text-align: center;
  vertical-align: middle;
  padding: 0.5rem;
}
.my-why {
  padding-bottom: 7rem;
  padding-top: 7rem;
  width: 100%;
  background-image: url("../assets/yellowskewed.svg");
  background-repeat: no-repeat;
  background-size:cover;
}
</style>
