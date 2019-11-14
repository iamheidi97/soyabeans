<template>
  <div class="my-footer footer-bg">

    <div class="row justify-content-center">
      <div class="col-lg-5 col-sm-12 text-left mx-sm-4 mb-sm-3 m-4">

        <h4 class="font-weight-bold text-center mb-3">Contact Us</h4>
        <div class="info row w-100">
          <i class="fa fa-phone fa-2x col-1"></i>
          <span class="ml-2">(032) 520 1039</span>
        </div>
        <div class="info row w-100">
          <i class="fa fa-envelope fa-2x col-1"></i>
          <span class="ml-2">info@soyabeansph.com</span>
        </div>
        <div class="info row w-100">
          <i class="fa fa-facebook-f fa-2x col-1"></i>
          <b-link class="f-link text-decoration-none ml-2" href="https://www.facebook.com/SoyaBeansPH/">www.facebook.com/SoyaBeansPH/</b-link>
          
        </div>
      </div>

      <div class="map-div col-lg-5 col-sm-12 align-self-end mx-sm-4">

        <div class="mapouter">
          <div class="gmap_canvas">
            <iframe
              id="gmap_canvas"
              src="https://maps.google.com/maps?q=Do%C3%B1a%20Luisa%20Bldg.%20%20%20%20Fuente%20Osme%C3%B1a%20Circle%20%20%20%20Cebu%20City%206000%2C%20Philippines&t=&z=13&ie=UTF8&iwloc=&output=embed"
              frameborder="0"
              scrolling="no"
              marginheight="0"
              marginwidth="0"
              height="100%"
              width="80%"
            ></iframe>
          </div>
        </div>
      </div>
    </div>

    <div class="foo d-block mt-4 pb-1">
      <h6>© 2017-2019 - www.soyabeansph.com</h6>
    </div>
  </div>
</template>
<script>

</script>
<style scoped>
.my-footer{
}

.footer-bg {
  background-image: linear-gradient(0deg, #fff1c6 50%, #ffffff 100%);
}
h4,h6 {
  color: #23a262;
}
.fa-envelope, .fa-phone, i.fa.fa{
  color: #23a262;
}
a{
  color: none;
}
.info {
  margin: 10px 0 0 0;
}

@media (max-width: 576px) {
    .f-link{font-size: 0.9em;}
    .info {
      font-size: 0.8em;
    }
}
</style>
