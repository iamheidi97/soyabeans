<template>
  <div class="my-faqs">
    <div class="row justify-content-center">
      <div class="col-lg-5 col-sm-11 m-3 m-sm-3">
        <div role="tablist">
          <h1 class="font-weight-bolder">FAQS</h1>
          <h2>Frequently Asked Questions</h2>

          <b-card no-body class="mt-5">
            <b-card-header header-tag="header" class role="tab">
              <b-button block href="#" v-b-toggle.accordion-1 variant="light">Who are my teachers?</b-button>
            </b-card-header>
            <b-collapse id="accordion-1" visible accordion="my-accordion" role="tabpanel">
              <b-card-body>
                <b-card-text>We have a native Japanese sensei that could help you learn Japanese language in an easy and enjoyable manner.</b-card-text>
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
                <b-card-text>When you finish a course in Soya Beans Language School, you can be given a certificate that proves the number of hours and the course you have undertaken with us.</b-card-text>
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
      <div class="ml-lg-5 col-lg-4 col-sm-11 align-self-end mt-sm-5 m-3 m-sm-3">
        <div role="tablist">
          <form class="p-5" @submit.prevent="handleSubmit">
            <h2 class="font-weight-bolder">BOOK YOUR FREE DEMO TODAY!</h2>
            <div class="form-group">
              <input type="text" class="form-control" id="name" placeholder="Name" v-model="book.userName"/>
              <div v-if="booked && !$v.book.userName.required" class="invalid-feedback">Name is required.</div>
            </div>
            <div class="form-group">
              <input type="number" class="form-control" id="phone" placeholder="Phone Number" v-model="book.userNumber"/>
              <div v-if="booked && !$v.book.userNumber.required" class="invalid-feedback">Contact Number is required.</div>
                    <div v-if="booked && !$v.book.userNumber.minLength" class="invalid-feedback">Contact number should only have 11 digits.</div>
                    <div v-if="booked && !$v.book.userNumber.maxLength" class="invalid-feedback">Contact number should only have 11 digits.</div>
              
            </div>
            <div class="form-group">
              <input
                type="email"
                class="form-control"
                id="email"
                aria-describedby="emailHelp"
                placeholder="Email Address"
                v-model="book.userEmail"
              />
              <div v-if="booked && !$v.book.userEmail.required" class="invalid-feedback">Email is required.</div>
              <div v-if="booked && !$v.book.userEmail.email" class="invalid-feedback">Email is invalid.</div>
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
    import { required,email,numeric,minLength,maxLength } from "vuelidate/lib/validators";
    
    export default {
      data() {
        return {
          booked: false,
          book: {
                    userName:"",
                    userEmail:"",
                    userNumber:"",
                }
        }
      },
      validations: {
            book: {
               userName: {required},
               userEmail: {required,email},
               userNumber: {required, numeric, minLength:minLength(11) , maxLength: maxLength(11)}
            }
      },
      methods: {
            handleSubmit(){
                this.booked = true;
                this.$v.$touch();
                if(this.$v.$invalid) {
                    return;
                }
                this.sendEmail();
            },
            showAlert(){
                this.$swal('Message sent!', 'We will get back to you as soon as possible','success');
            },
            clearFields(){
                this.book.userName = ""
                this.book.userNumber = ""
                this.book.userEmail = ""
            },
            sendEmail() {
                window.Email.send({
                    SecureToken : "75c4abd2-34bc-49e8-bff2-d163131d0e38",
                    To : 'info@soyabeansph.com',
                    From : "lenej@windsgate.com",
                    Subject : this.book.userName + ' ' + "is interested for a free demo from Soya Beans",
                    Body : "This person is interested for a free demo from Soya Beans. Please contact him/her as soon as possible." + "<br><strong>Name:</strong> " + this.book.userName + "<br><strong>Email:</strong> " + this.book.userEmail + "<br><strong>Contact Number:</strong> " + this.book.userNumber
                }).then( () => 
                    {
                        this.showAlert();
                        this.clearFields();
                    }   
                );
            }
        },
    }
</script>
<style scoped>
    .invalid-feedback {
      display: block;
    }
    .my-faqs {
      margin-top: 10em;
      margin-bottom: 7em;
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
