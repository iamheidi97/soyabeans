<template>
  <div class="my-header header-bg border-bottom-solid">
    <b-navbar toggleable="lg">
      <img class="img-responsive mr-2" id="nav-logo" src="../assets/soyalogo.png" />
      <label class="h-title font-weight-bold mr-auto" href="#">Soya Beans Japanese Language School</label>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-auto">
          <b-nav-item href="#home" class="hvr-underline-from-center mr-3 my-2">Home</b-nav-item>
          <b-nav-item href="#why" class="hvr-underline-from-center mr-3 my-2">Why Choose Us</b-nav-item>
          <b-nav-item href="#courses" class="hvr-underline-from-center mr-3 my-2">Courses</b-nav-item>
          <b-nav-item href="#faqs" class="hvr-underline-from-center mr-3 my-2">FAQS</b-nav-item>
          <b-nav-item href="#contact" class="hvr-underline-from-center mr-3 my-2">Contact Us</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>
<script>
</script>
<style scoped>
.my-header {
  color: #54aa67;
  box-sizing: border-box;
}
label {
  padding: 0;
}
.header-bg {
  background-image: linear-gradient(90deg, #f2ffed 50%, #99e7a3 100%);
}
label.h-title {
  font-size: 1.25rem;
  margin: 0;
}
a.nav-link:hover {
  display: inline-block;
  vertical-align: middle;
  -webkit-transform: perspective(1px) translateZ(0);
  transform: perspective(1px) translateZ(0);
  box-shadow: 0 0 0.1px rgba(0, 0, 0, 0);
  position: relative;
  overflow: hidden;
}
#nav-logo {
  height: 60px;
}
/* Underline From Center */
.hvr-underline-from-center {
  display: inline-block;
  vertical-align: middle;
  -webkit-transform: perspective(1px) translateZ(0);
  transform: perspective(1px) translateZ(0);
  /* box-shadow: 0 0 .1px rgba(0, 0, 0, 0); */
  position: relative;
  overflow: hidden;
}
.hvr-underline-from-center:before {
  content: "";
  position: absolute;
  z-index: -1;
  left: 51%;
  right: 51%;
  bottom: 0;
  background: #54aa67;
  height: 4px;
  -webkit-transition-property: left, right;
  transition-property: left, right;
  -webkit-transition-duration: 0.3s;
  transition-duration: 0.3s;
  -webkit-transition-timing-function: ease-out;
  transition-timing-function: ease-out;
}
.hvr-underline-from-center:hover:before,
.hvr-underline-from-center:focus:before,
.hvr-underline-from-center:active:before {
  left: 0;
  right: 0;
}

.navbar-light .navbar-nav .nav-link {
  font-weight: bold;
  color: rgba(84, 170, 103, 1);
}
</style>
