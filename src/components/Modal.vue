<template>
  <div>
    <b-button variant="success" @click="show=true" class="mt-5 p-3" size="lg">
        <div class="row justify-content-center">
          <div class="col-12 col-sm-12 col-md-2 "><i class="m-icon fa fa-envelope fa-2x"></i></div>
          <div class="col-12 col-sm-12 col-md-10 align-self-center">Get in touch with us</div>
        </div>
        
    </b-button>
    <b-modal id="myModal" v-model="show" centered>
      <template v-slot:modal-title>
        <h4 class="font-weight-bolder green-text">Interested? Get in touch with Soya Beans!</h4>
      </template>
      <form class="p-3" @submit.prevent="handleSubmit">
        <div class="form-group">
          <input
            type="text"
            class="form-control"
            id="userName"
            placeholder="Name"
            :class="{ 'is-invalid': submitted && $v.userMessage.userName.$error }"
      
      
            v-model="userMessage.userName"
          />
          <div
            v-if="submitted && !$v.userMessage.userName.required"
            class="invalid-feedback"
          >Name is required.</div>
        </div>
        <div class="form-group">
          <!-- <label for="exampleInputEmail1">Email address</label> -->
          <input
            type="email"
            class="form-control"
            id="userEmail"
            aria-describedby="emailHelp"
            placeholder="Email"
            :class="{ 'is-invalid': submitted && $v.userMessage.userEmail.$error }"
            v-model="userMessage.userEmail"
          />
          <div
            v-if="submitted && !$v.userMessage.userEmail.required"
            class="invalid-feedback"
          >Email is required.</div>
          <div
            v-if="submitted && !$v.userMessage.userEmail.email"
            class="invalid-feedback"
          >Email is invalid.</div>
        </div>
        <div class="form-group">
          <!-- <label for="exampleInputPassword1">Password</label> -->
          <input
            type="number"
            class="form-control"
            id="userNumber"
            placeholder="Contact Number"
            :class="{ 'is-invalid': submitted && $v.userMessage.userNumber.$error }"
            v-model="userMessage.userNumber"
          />
          <div
            v-if="submitted && !$v.userMessage.userNumber.required"
            class="invalid-feedback"
          >Contact Number is required.</div>
          <div
            v-if="submitted && !$v.userMessage.userNumber.minLength"
            class="invalid-feedback"
          >Contact number should only have 11 digits.</div>
          <div
            v-if="submitted && !$v.userMessage.userNumber.maxLength"
            class="invalid-feedback"
          >Contact number should only have 11 digits.</div>
        </div>
        <div class="form-group">
          <textarea
            class="form-control"
            id="userMessage"
            rows="6"
            placeholder="Please enter your message"
            style="overflow:auto;resize:none"
            :class="{ 'is-invalid': submitted && $v.userMessage.userMessage.$error }"
            v-model="userMessage.userMessage"
          ></textarea>
          <div
            v-if="submitted && !$v.userMessage.userMessage.required"
            class="invalid-feedback"
          >Message is required.</div>
        </div>
        <input type="submit" id="submit-form" class="d-none" />
      </form>
      <template v-slot:modal-footer>
        <div class="w-100">
          <div class="float-right">
            <b-button class="mr-1" variant="outline-secondary" size="md" @click="show=false">Close</b-button>
            <label for="submit-form" tabindex="0" class="btn btn-success btn-md my-1">Send Message</label>
            <!-- <b-button
                            variant="success"
                            size="md"
                            @click="show=false" 
                        >
                            Send Message
            </b-button>-->
          </div>
        </div>
      </template>
    </b-modal>
  </div>
</template>

<script>
import {
  required,
  email,
  numeric,
  minLength,
  maxLength
} from "vuelidate/lib/validators";
export default {
  mounted() {},
  data() {
    return {
      show: false,
      submitted: false,
      userMessage: {
        userName: "",
        userEmail: "",
        userNumber: "",
        userMessage: ""
      }
    };
  },
  validations: {
    userMessage: {
      userName: { required },
      userEmail: { required, email },
      userNumber: {
        required,
        numeric,
        minLength: minLength(11),
        maxLength: maxLength(11)
      },
      userMessage: { required }
    }
  },
  methods: {
    handleSubmit() {
      this.submitted = true;
      this.$v.$touch();
      if (this.$v.$invalid) {
        return;
      }
      this.sendEmail();
    },
    showAlert() {
      this.$swal(
        "Message sent!",
        "We will get back to you as soon as possible",
        "success"
      );
    },
    sendEmail() {
      window.Email.send({
        SecureToken: "75c4abd2-34bc-49e8-bff2-d163131d0e38",
        To: "info@soyabeansph.com",
        From: "lenej@windsgate.com",
        Subject: "New message from Soya Beans website",
        Body:
          "<strong>Name:</strong> " +
          this.userMessage.userName +
          "<br><strong>Email:</strong> " +
          this.userMessage.userEmail +
          "<br><strong>Contact Number:</strong> " +
          this.userMessage.userNumber +
          "<br><strong>Message</strong>: " +
          this.userMessage.userMessage
      }).then(() => {
        this.$bvModal.hide("myModal");
        this.showAlert();
      });
    }
  }
};
</script>

<style>
.m-icon{
    height: 1px;
}
.modal-header {
  border-bottom: 1px solid #4fb581;
}
.modal-footer {
  border-top: none;
}
</style>