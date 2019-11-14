<template>
  <div>
    <Header id="header" class="higher-z"/>
    <Home id="home" class="upperslight1"/>
    <Why id="why"/>
    <Testimonies id="testimonies"/>
    <Courses id="courses"/>
    <Faqs id="faqs"/>
    <Footer id="contact"/>
    <go-top bg-color="#23A262" fg-color="#FFFBE5"></go-top>
  </div>
</template>
<script>
import Header from "./Header"
import Home from "./Home";
import Why from "./Why";
import Testimonies from "./Testimonies";
import Courses from "./Courses";
import Faqs from "./Faqs";
import Footer from "./Footer";
import GoTop from '@inotom/vue-go-top';

export default {
  components: {
    GoTop,
    Header,
    Home,
    Why,
    Testimonies,
    Courses,
    Faqs,
    Footer
  }
};
</script>
<style scoped>
/* @import url("https://fonts.googleapis.com/css?family=Montserrat&display=swap"); */
@import url("https://fonts.googleapis.com/css?family=Montserrat:400,600,700,800,900&display=swap");

  body {
    font-family: "Montserrat", sans-serif !important;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    overflow: hidden;
  }
  .upperslight1 {
    position: relative;
    margin-top: -5%;
    z-index: 100;
  }
  .higher-z {
    position: relative;
    z-index: 1000;
  }
</style>

