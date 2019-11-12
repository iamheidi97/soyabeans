<template>
    <div class="">
        <Header/>
        <Home/>
        <SoyaDescription/>
        <Why/>
        <Testimonies />
        <Courses/>
        <Faqs/>
        <Footer/>
    </div>
</template>
<script>
import Header from './Header'
import Home from './Home'
import SoyaDescription from './SoyaDescription'
import Why from './Why'
import Testimonies from './Testimonies'
import Courses from './Courses'
import Faqs from './Faqs'
import Footer from './Footer'

export default {
  components: {
      Header,
      Home,
      SoyaDescription,
      Why,
      Testimonies,
      Courses,
      Faqs,
      Footer
  }
}
</script>
<style>
/* @import url("https://fonts.googleapis.com/css?family=Montserrat&display=swap"); */
@import url('https://fonts.googleapis.com/css?family=Montserrat:400,600,700,800,900&display=swap');

    body {
        font-family: "Montserrat", sans-serif !important;
    }

</style>
