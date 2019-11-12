<template>
  <div class="my-footer footer-bg ">
    <div class="contact">
      <i class="fas fa-phone-alt"></i>
    </div>
    <div class="my-map">
      <div class="mapouter">
        <div class="gmap_canvas">
          <iframe
            id="gmap_canvas"
            src="https://maps.google.com/maps?q=Do%C3%B1a%20Luisa%20Bldg.%20%20%20%20Fuente%20Osme%C3%B1a%20Circle%20%20%20%20Cebu%20City%206000%2C%20Philippines&t=&z=13&ie=UTF8&iwloc=&output=embed"
            frameborder="0"
            scrolling="no"
            marginheight="0"
            marginwidth="0"
            height="200px"
            width="500px"
          ></iframe>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
</script>
<style scoped>
.my-footer{
  position: relative;
  bottom: 0;
}
.footer-bg{
  background-image: linear-gradient(0deg, #fff1c6 50%, #ffffff 100%);
}
</style>
