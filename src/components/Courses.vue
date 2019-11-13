<template>
  <div class="my-courses m-5">
    <div class="my-5">
      <label class="font-weight-bolder display-4 green-text">Courses Available</label>
    </div>
    <div class="container-fluid">
      
      <div class="row justify-content-center">
        <div class="col-11">
          <p
            class="text-left"
          >With our experienced native Japanese instructor she will support your learning to widen your career opportunity and unlock one of the world's largest economy and its distinctive culture.</p>
          <p class="text-left">We also cater one-on-one or group classes.</p>
        </div>
      </div>
    </div>

    <div class="mt-3">
      <div class="row justify-content-center">
        <div class="col-xl-3 col-lg-3 col-md-6 col-xs-12 align-self-top pb-sm-3 pb-3">
          <b-card border-variant="light" class="text-center h-100">
            <template v-slot:header>
              <small class="text-muted">Beginner</small>
              <h2 class="mb-0 my-3 font-weight-bold">
                Tourist / Travel
                <br />Course
              </h2>
            </template>
            <b-card-text class="px-4">
              <p>Planning to visit Japan? Know Enough Japanese to get around Japan and interact with the locals.</p>
              <p>You will be taught the basic writing conventions (Hiragana and Katakana) and useful expressions in Japanese. You willalso be given insights on the Japanese culture.</p>
            </b-card-text>
            <template v-slot:footer>
              <p class="my-3">
                2-hour sessions
                <br />every Wednesday & Friday
                <br />for 4 weeks
                <br />
              </p>
            </template>
          </b-card>
        </div>

        <div class="col-xl-3 col-lg-3 col-md-6 col-xs-12 align-self-top pb-sm-3 pb-3">
          <b-card border-variant="light" class="text-center h-100">
            <template v-slot:header>
              <small class="text-muted">Beginner to Intermediate</small>
              <h2 class="mb-0 my-3 font-weight-bold">
                Hobbyist / Otaku
                <br />Course
              </h2>
            </template>
            <b-card-text class="px-4">
              <p>Do you admire Japan's culture? Or do you want to watch ani,e or manga without having to wait for subtitles? This course is for you.</p>
              <p>Conversational Japnese will be taught to you. Test your Japanese and immerse yourself by reading our wide ccollection of mangas and anime related materials.</p>
            </b-card-text>
            <template v-slot:footer>
              <p class="my-3">
                1.5-hour sessions
                <br />every Tuesday & Thursday
                <br />for 4 weeks
                <br />
              </p>
            </template>
          </b-card>
        </div>
        <div class="col-xl-3 col-lg-3 col-md-6 col-xs-12 pb-sm-3 pb-3">
          <b-card border-variant="light" class="text-center h-100">
            <template v-slot:header>
              <small class="text-muted">Beginner to Intermediate</small>
              <h2 class="mb-0 my-3 font-weight-bold">
                Business
                <br />Course
              </h2>
            </template>
            <b-card-text class="px-4">
              <p>Dealing with Japanese clients most of the time? Impress them with your Japanese with this course.</p>
              <p>Learn how to speak and write formally in Japanese, the do's and dont's when dealing with Japanese clients and more.</p>
            </b-card-text>
            <template v-slot:footer>
              <p class="my-3">
                Schedules may be flexible.
                <br />Please contact us
                <br />for consultation.
                <br />
              </p>
            </template>
          </b-card>
        </div>

        <div class="col-xl-3 col-lg-3 col-md-6 col-xs-12 pb-sm-3 pb-3">
          <b-card border-variant="light" class="text-center h-100">
            <template v-slot:header>
              <small class="text-muted">Beginner to Advanced</small>
              <h2 class="mb-0 my-3 font-weight-bold">
                JLPT
                <br />Course
              </h2>
            </template>
            <b-card-text class="px-4">
              <p>Do you already have plans to go to work to Japan? Certification exams increase your chances of achieving those dreams.</p>
              <p>You will be taught Japanese in accordance to the strucutre of the JLPT Exams. Test yourself with mock tests that will be provided to assessyour Japanese.</p>
              <p>
                <strong>N5, N4, N5+N4, N3, and N2</strong> courses are available.
              </p>
            </b-card-text>
            <template v-slot:footer>
              <p class="my-3">
                2-hour sessions
                <br />every Tuesday & Thursday
                <br />for 12 weeks
              </p>
            </template>
          </b-card>
        </div>
      </div>
    </div>
    <b-button
      type="button"
      class="btn btn-primary btn-lg p-3 my-5"
      variant="success"
    >Get in touch with us</b-button>
  </div>
</template>
<script>
</script>
<style scoped>
    @media (max-width: 576px) {
          .display-4 {
            font-size: 2.8rem;
          }
          h2 {
            font-size: 1.9rem;
          }
        }
small {
  font-size: 70%;
}
.my-courses {
  box-sizing: border-box;
  overflow: hidden;
  margin-top: 5em;
  margin-bottom: 5em;
}

div.card-header {
  font-size: 20px;
  font-weight: bolder;
  color: #158c39;
}
div.card-body,
div.card-header {
  background-color: #fffbe5;
  border-bottom: none;
}
.card-footer {
  border-top: none;
  font-weight: bolder;
  color: #158c39;
  background-color: rgba(40, 167, 69, 0.1);
}
.card-foo {
  font-weight: bolder;
  color: #158c39;
  bottom: 0;
}
.btn-lg {
  font-size: 1.6rem;
}
/* label {
  font-size: 5vw;
} */
.div.col{
  padding-right: 0; 
}
</style>
