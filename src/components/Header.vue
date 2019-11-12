<template>
  <div class="my-header">



    <nav class="navbar navbar-expand-lg header-bg">
      <div>
        <a class="navbar-brand d-none d-md-inline">
        <img class="img-responsive mr-2" id="nav-logo" src="../assets/soyalogo.png" />
        <label class="h-title font-weight-bold">Soya Beans Japanese Language School</label>
      </a>
      </div>

      
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-auto mr-4">
          <b-nav-item href="#" class="hvr-underline-from-center mr-3">Home</b-nav-item>
          <b-nav-item href="#" class="hvr-underline-from-center mr-3">Why Choose Us</b-nav-item>
          <b-nav-item href="#" class="hvr-underline-from-center mr-3">Courses</b-nav-item>
          <b-nav-item href="#" class="hvr-underline-from-center mr-3">FAQS</b-nav-item>
          <b-nav-item href="#" class="hvr-underline-from-center mr-3">Contact Us</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
      <b-navbar/>
    </nav>
  </div>
</template>
<script>
</script>
<style scoped>
    @import url("https://fonts.googleapis.com/css?family=Montserrat&display=swap");

    .my-header {
      font-family: "Montserrat", sans-serif;
    }
    #nav-logo {
      height: 60px;
    }
    a.nav-link{
      /* margin-left: 1.1rem; */
      color: #54aa67;
      font-weight: bold;
    }
    /* a.nav-link:hover{
      transition: all 0.3s ease 0s;
      color: #2c3e50;
      font-size: 18px;
    } */
    .h-title{
      color: #54aa67;
    }
    .header-bg {
      background-image: linear-gradient(90deg, #f2ffed 50%, #99e7a3 100%);
      /* filter: blur(8px);
      -webkit-filter: blur(1px);
      z-index: -1; */
    }
    .bg-blur {
      /* Add the blur effect */
        filter: blur(8px);
        -webkit-filter: blur(8px);

        /* Full height */
        height: 100%;
    }
    a.btn.button{
      font-weight: bold;
      color: #1e5707;
      border-radius: 2rem;
    }
    a:hover{
      color: #54aa67;
    }
    /* Underline From Center */
    .hvr-underline-from-center {
      display: inline-block;
      vertical-align: middle;
      -webkit-transform: perspective(1px) translateZ(0);
      transform: perspective(1px) translateZ(0);
      box-shadow: 0 0 1px rgba(0, 0, 0, 0);
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
    .hvr-underline-from-center:hover:before, .hvr-underline-from-center:focus:before, .hvr-underline-from-center:active:before {
      left: 0;
      right: 0;
    }



</style>
