<template>
  <div class="my-faqs mx-5">
    <div class="row justify-content-center">
      <div class="col-5">
        <div role="tablist">
          <h1 class="font-weight-bolder">FAQS</h1>
          <h2>Frequently Asked Questions</h2>

          <b-card no-body class="mt-5">
            <b-card-header header-tag="header" class role="tab">
              <b-button block href="#" v-b-toggle.accordion-1 variant="light">Who are my teachers?</b-button>
            </b-card-header>
            <b-collapse id="accordion-1" visible accordion="my-accordion" role="tabpanel">
              <b-card-body>
                <b-card-text>We have a native japanese sensei that could help you learn Japanese language in an easy and enjoyable manner.</b-card-text>
              </b-card-body>
            </b-collapse>
          </b-card>

          <b-card no-body class>
            <b-card-header header-tag="header" class role="tab">
              <b-button
                block
                href="#"
                v-b-toggle.accordion-2
                variant="light"
              >Do I get a certificate at the end of my course?</b-button>
            </b-card-header>
            <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
              <b-card-body>
                <b-card-text>When you finish a course in Soya beanss language School, you can be given a certificate that proves that you have undertaken that course with us.</b-card-text>
              </b-card-body>
            </b-collapse>
          </b-card>

          <b-card no-body class>
            <b-card-header header-tag="header" class role="tab">
              <b-button
                block
                href="#"
                v-b-toggle.accordion-3
                variant="light"
              >Can I enroll a course as an absolute beginner?</b-button>
            </b-card-header>
            <b-collapse id="accordion-3" accordion="my-accordion" role="tabpanel">
              <b-card-body>
                <b-card-text>Yes, absolutely! You may contact us if you are interested in such course.</b-card-text>
              </b-card-body>
            </b-collapse>
          </b-card>

          <b-card no-body class>
            <b-card-header header-tag="header" class role="tab">
              <b-button
                block
                href="#"
                v-b-toggle.accordion-4
                variant="light"
              >I am busy. Can I have a different schedule instead?</b-button>
            </b-card-header>
            <b-collapse id="accordion-4" accordion="my-accordion" role="tabpanel">
              <b-card-body>
                <b-card-text>
                  Of course! you may
                  <b>contact us</b> so that we can tailor a schedule fit for your needs.
                </b-card-text>
              </b-card-body>
            </b-collapse>
          </b-card>
        </div>
      </div>
      <div class="ml-5 col-4 align-self-center">
        <div role="tablist">
          <form class="p-5">
            <h2 class="font-weight-bolder">BOOK YOUR FREE DEMO TODAY</h2>
            <div class="form-group">
              <input type="text" class="form-control" id="name" placeholder="Name" />
            </div>
            <div class="form-group">
              <input type="number" class="form-control" id="phone" placeholder="Phone Number" />
            </div>
            <div class="form-group">
              <input
                type="email"
                class="form-control"
                id="email"
                aria-describedby="emailHelp"
                placeholder="Email Address"
              />
            </div>
            <div>
              <button type="submit" class="btn btn-success">S U B M I T</button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
</script>
<style scoped>
    .my-faqs {
      height: 100vh;
    }
    form {
      background-color: #fffbe5;
    }
    h2,
    h1 {
      color: #23A262;
    }
    .btn {
      width: 100%;
      margin: 20px 0;
    }
    .form-group {
      margin: 15px 0;
    }
    header.card-header {
      background-color: #fffbe5;
      padding: 0;
      margin: 0;
      border: none;
    }
    a.btn {
      color: #23A262;
      font-weight: bold;
      border: none;
      outline: none;
      background-color: #fffbe5;
    }
    a.btn:focus {
      border: none;
      outline: none;
      box-shadow: none;
    }
    input[type=number]::-webkit-inner-spin-button, 
    input[type=number]::-webkit-outer-spin-button { 
      -webkit-appearance: none; 
      margin: 0; 
    }
    .card {
      border: 1px solid #FFFBE5;
    }
    .btn {
      font-size: 1.2em;
    }
</style>
