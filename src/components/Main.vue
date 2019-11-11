<template>
    <div>
        <Header/>
        <Home/>
        <SoyaDescription/>
        <Courses/>
        <Why/>
        <Footer/>
    </div>
</template>
<script>
import Header from './Header'
import Home from './Home'
import SoyaDescription from './SoyaDescription'
import Why from './Why'
import Courses from './Courses'
import Footer from './Footer'

export default {
  components: {
      Header,
      Home,
      SoyaDescription,
      Why,
      Courses,
      Footer
  }
}
</script>
<style>
    body {
        font-style: Montserrat, sans-serif !important;
    }

</style>
