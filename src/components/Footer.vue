<template>
  <div class="my-footer footer-bg">

    <div class="row justify-content-center">
      <div class="col-lg-3 col-sm-6 align-top mt-5 text-left mx-sm-4 mb-sm-3">
        <h4 class="font-weight-bold text-center mb-3">Contact Us</h4>
        <div class="info">
          <i class="fa fa-phone fa-2x mr-2"></i>text
          <span>(032) 520 1039</span>
        </div>
        <div class="info justify-content-center">
          <i class="fa fa-envelope fa-2x mr-2"></i>
          <span class="ml-auto">info@soyabeansph.com</span>
        </div>
        <div class="info">
          
          <b-link href="www.facebook.com/SoyaBeansPH/"><i class="fa fa-facebook-f fa-2x mr-2"></i>www.facebook.com/SoyaBeansPH/</b-link>
        </div>
      </div>
      <div class="col-lg-3 col-sm-11 my-map align-self-end mx-sm-4">
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
              width="100%"
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
body{
  margin: 0;
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
</style>
