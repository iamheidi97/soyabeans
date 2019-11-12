<template>
  <div class="my-header">
    <nav class="nav navbar navbar-expand-lg header-bg">
      <div>
        <a class="navbar-brand d-none d-md-inline">
        <img class="img-responsive mr-2" id="nav-logo" src="../assets/soyalogo.png" />
        <label class="h-title font-weight-bold">Soya Beans Japanese Language School</label>
      </a>
      </div>
      
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-auto mr-4">
          <b-nav-item href="#">Home</b-nav-item>
          <b-nav-item href="#">Why Choose Us</b-nav-item>
          <b-nav-item href="#">Courses</b-nav-item>
          <b-nav-item href="#">FAQS</b-nav-item>
          <b-button href="#" class="button ml-4 mr-0" variant="warning">Contact Us</b-button>
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
  margin-left: 1.1rem;
  color: #54aa67;
  font-weight: bold;
}
a.nav-link:hover{
  transition: all 0.3s ease 0s;
  color: #2c3e50;
  font-size: 18px;
}
.h-title{
  color: #54aa67;
}
.header-bg {
background-image: linear-gradient(90deg, #f2ffed 50%, #99e7a3 100%);
}
a.btn.button{
  font-weight: bold;
  color: #1e5707;
  border-radius: 2rem;
}
</style>
