<template>
  <div id="app">
    
    <Main />
    <back-to-top text="Back to top">
      <button type="button" class="btn btn-success btn-to-top"><i class="fa fa-chevron-up"></i></button>
    </back-to-top>
  </div>
</template>

<script>
import Main from "./components/Main.vue";


export default {
  name: "app",
  components: {
    Main
  },
  mounted() {
    let smtpJsScript = document.createElement('script');
            smtpJsScript.setAttribute('src', 'https://smtpjs.com/v3/smtp.js'); 
            smtpJsScript.defer = true
            document.head.appendChild(smtpJsScript);
  },
};
</script>

<style>
#app {
  font-size: 16px;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  box-sizing: border-box;
  overflow: hidden;
  padding: 0;
  margin: 0;
  color: #23A262;
}
/* html{
  scroll-behavior:smooth
  } */
.btn-to-top {
  /* width: 60px;
  height: 60px;
  padding: 10px 16px;
  border-radius: 50%; */
  font-size: 1.3em;
  line-height: 0.9em;
  padding: 1rem;
  background-color: #23A262;

}
.btn-success {
  background-color: #23a262;
  border-color: #23a262;
}
.green-text {
  color: #23a262;
}
@import url("https://fonts.googleapis.com/css?family=Montserrat:400,600,700,800,900&display=swap");

body {
  font-family: "Montserrat", sans-serif !important;
  padding: 0;
}

  @media (max-width: 576px) {
      .display-4 {
        font-size: 2.8rem;
      }
  }

  /* // Medium devices (tablets, 768px and up) */
  @media (max-width: 768px) {  }

  /* // Large devices (desktops, 992px and up) */
  @media (min-width: 992px) {  }

  /* // Extra large devices (large desktops, 1200px and up) */
  @media (min-width: 1200px) { }

</style>
