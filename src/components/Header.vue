<template>
  <div class="my-header border-bottom-solid">
    <!-- <HeaderBg/> -->
    <b-navbar toggleable="lg">
      <img class="my-logo img-responsive mr-2" id="nav-logo" src="../assets/soyalogo.png" />
      <label class="h-title text1 font-weight-bold mr-auto d-sm-none d-lg-block d-none" href="#">Soya Beans Japanese Language School</label>
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
  
  
  export default {
    // components: {
    //   Name
    // },
    mounted() {
      document.querySelectorAll('a[href^="#"]').forEach(anchor => {
          anchor.addEventListener('click', function (e) {
              e.preventDefault();

              document.querySelector(this.getAttribute('href')).scrollIntoView({
                  behavior: 'smooth'
              });
          });
      });
          },
  }
</script>
<style scoped>
@supports (-webkit-backdrop-filter: none) or (backdrop-filter: none) {
  nav {
    -webkit-backdrop-filter: blur(16px);
    backdrop-filter: blur(16px);
    /* background-color: rgba(200, 200, 200, 0.2);   */
    background-color: rgba(40, 167, 69, 0.1);
    
  }
}
@media (max-width: 576px) {
    .navbar-light .navbar-nav .nav-link {
      font-weight: bold;
      /* color: #54aa67; */
      color: #23A262 !important;
    }
}
.my-logo{
  background-color: #fff9ba;
  border-radius: 100%;
  box-shadow: 3px 2px 0px #4f9e37;
}
.my-header {
  position: fixed;
  box-sizing: border-box;
  overflow: hidden;
}
label {
  padding: 0;
}
/* nav {
  background-color: #fff;
} */
label.h-title {
  font-size: 1.25rem;
  margin: 0;
  color: #fff9ba;
  text-shadow: 3px 2px 0px #4f9e37;
}
a.nav-link:hover {
  display: inline-block;
  vertical-align: middle;
  -webkit-transform: perspective(1px) translateZ(0);
  transform: perspective(1px) translateZ(0);
  color: #23A262;
  /* box-shadow: 0 0 0.1px rgba(0, 0, 0, 0); */
  position: relative;
  overflow: hidden;
}
#nav-logo {
  height: 2.8rem;
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
  background: #DCFFCC;
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
  /* color: #54aa67; */
  color: #DCFFCC;
}
.nav-link:hover{                           
  color: #DCFFCC !important;
}   

</style>
