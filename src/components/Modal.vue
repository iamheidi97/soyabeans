<template>
    <div>
        <b-button variant="success" @click="show=true" class="mt-5 p-3" size="lg">Get in touch with us</b-button>
        <b-modal id="myModal" v-model="show" centered >
            <template v-slot:modal-title>
                <h4 class="font-weight-bolder green-text">Interested? Get in touch with Soya Beans!</h4>
            </template>
            <form class="p-3">
                <div class="form-group">
                    <input type="text" class="form-control" id="userName" placeholder="Name" :class="{ 'is-invalid': submitted && $v.userMessage.userName.$error }">
                </div>
                <div class="form-group">
                    <!-- <label for="exampleInputEmail1">Email address</label> -->
                    <input type="email" class="form-control" id="userEmail" aria-describedby="emailHelp" placeholder="Email"  :class="{ 'is-invalid': submitted && $v.userMessage.userEmail.$error }">
                </div>
                <div class="form-group">
                    <!-- <label for="exampleInputPassword1">Password</label> -->
                    <input type="number" class="form-control" id="userNumber" placeholder="Contact Number"  :class="{ 'is-invalid': submitted && $v.userMessage.userNumber.$error }">
                </div>
                <div class="form-group">
                    <textarea class="form-control" id="userMessage" rows="6" placeholder="Please enter your message" style="overflow:auto;resize:none" :class="{ 'is-invalid': submitted && $v.userMessage.userMessage.$error }"></textarea>
                </div>
                <input type="submit" id="submit-form" class="hidden" />
            </form>
                <template v-slot:modal-footer>
                    <div class="w-100">
                        <div class="float-right">
                            <b-button
                            class="mr-1"
                            variant="outline-secondary"
                            size="md"
                            @click="show=false"
                        >
                            Close
                        </b-button>
                        <label for="submit-form" tabindex="0" class="btn btn-success btn-md" @click="show=false">Send Message</label>
                        <!-- <b-button
                            variant="success"
                            size="md"
                            @click="show=false" 
                        >
                            Send Message
                        </b-button> -->
                        </div>
                    </div>
                </template>
        </b-modal>
    </div>
</template>

<script>
    import { required,email,numeric,minLength,maxLength } from "vuelidate/lib/validators";
    export default {
        data() {
            return {
                show: false,
                submitted: false,
                userMessage: {
                    userName:"",
                    userEmail:"",
                    userNumber:"",
                    userMessage:""
                }
                
            }
        },
        validations: {
            userMessage: {
                userName: { required },
                userEmail: { required, email},
                userNumber: { required, numeric, minLength:minLength(11) , maxLength: maxLength(11)},
                userMessage: { required }
            }
        },
        methods: {
            handleSubmit(){
                this.submitted = true;
                this.$v.touch();
                if(this.$v.invalid) {
                    return;
                }
                alert("Message sent!");
            }
        },
    }
</script>

<style>
    .modal-header {
        border-bottom: 1px solid #4FB581;
    }
    .modal-footer {
        border-top: none;
    }
</style>