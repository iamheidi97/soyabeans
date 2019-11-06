<template>
    <div>
        <Header/>
        <Home/>
        <Courses/>
        <Why/>
        <Footer/>
    </div>
</template>
<script>
import Header from './Header'
import Home from './Home'
import Why from './Why'
import Courses from './Courses'
import Footer from './Footer'

export default {
  components: {
      Header,
      Home,
      Why,
      Courses,
      Footer
  }
}
</script>
<style>

</style>
