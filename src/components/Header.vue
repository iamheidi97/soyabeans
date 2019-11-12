<template>
  <div class="my-header">
    <nav class="navbar navbar-expand-lg dusty-grass-gradient border-bottom">
      <div>
        <a class="navbar-brand d-none d-md-inline">
        <img class="img-responsive mr-2" id="nav-logo" src="../assets/soyalogo.png" />
        <label class="h-title font-weight-bold">Soya Beans Japanese Language School</label>
      </a>
      </div>
      
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-auto mr-5">
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
a.nav-link{
  margin-left: 1rem;
  color: #54aa67;
  font-weight: bold;
}
a.nav-link :hover{
  transition: all 0.3s ease 0s;
  color: yellow;
  text-decoration: underline;
  size: 3rem;
}
.h-title{
  color: #54aa67;
}

</style>
