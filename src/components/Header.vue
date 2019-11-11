<template>
  <div class="my-header">
    <nav class="navbar navbar-expand-lg navbar-light bg-lightgreen border-bottom">
      <div>
        <a class="navbar-brand d-none d-md-inline">
        <img class="img-responsive mr-2" id="nav-logo" src="../assets/soyalogo.png" />
        <label class="font-weight-bold">Soya Beans Japanese Language School</label>
      </a>
      </div>
      
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-auto font-weight-bold mr-5">
          <b-nav-item href="#">Home</b-nav-item>
          <b-nav-item href="#">Why Choose Us</b-nav-item>
          <b-nav-item href="#">Courses</b-nav-item>
          <b-nav-item href="#">FAQS</b-nav-item>
          <b-nav-item href="#">Contact Us</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
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
a{
  margin-left: 1rem;
}
</style>
