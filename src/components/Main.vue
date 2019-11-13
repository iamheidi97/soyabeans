<template>
  <div>
    <Header1 id="header"/>
    <Home id="home"/>
    <Why id="why"/>
    <Testimonies id="testimonies"/>
    <Courses id="courses"/>
    <Faqs id="faqs"/>
    <Footer id="contact"/>
  </div>
</template>
<script>
import Header1 from "./Header1"
import Home from "./Home";
import Why from "./Why";
import Testimonies from "./Testimonies";
import Courses from "./Courses";
import Faqs from "./Faqs";
import Footer from "./Footer";

export default {
  components: {
    Header1,
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
}
</style>

