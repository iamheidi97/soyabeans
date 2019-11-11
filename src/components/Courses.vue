<template>
  <div class="my-courses m-5">
    <div class="my-5">
      <h1 class="font-weight-bolder display-4">Courses Available</h1>
    </div>
    <div class="container-fluid">
      <div class="row justify-content-center">
        <div class="col-11">
          <p class="text-left">With our experienced native Japanese instructor she will support your learning to widen your career opportunity and unlock one of the world's largest economy and its distinctive culture.</p>
          <p class="text-left">We also cater one-on-one or group classes.</p>
        </div>
      </div>
    </div>
    <div class="mt-3">
      <div class="row justify-content-center">
        <div class="col-3">
          <b-card border-variant="light" header="Tourist/Travel Course" class="text-center h-100">
            <b-card-text><small>Beginner</small></b-card-text>
            <b-card-text> 
              <p>Planning to visit Japan? Know Enough japanese to get around Japan and interact with the locals.</p>
              <p>You will be taught the basic writing conventions (Hiragana and Katakana) and useful expressions in Japanese. You willalso be given insights on the Japanese culture.</p>
            </b-card-text>
            <template v-slot:footer>
                <em>2-hour sessions every Wednesday & Friday <br>for 4 weeks<br></em>
            </template>
          </b-card>
        </div>
        <div class="col-3">
          <b-card border-variant="light" header="Hobbyist/Otaku Course" class="text-center h-100">
            <b-card-text><small>Beginner to Intermediate</small></b-card-text>
            <b-card-text>
              <p>Do you admire Japan's culture? Or do you want to watch ani,e or manga without having to wait for subtitles? This course is for you.</p>
              <p>Conversational Japnese will be taught to you. Test your Japanese and immerse yourself by reading our wide ccollection of mangas and anime related materials.</p>
            </b-card-text>
            <template v-slot:footer>
                <em>1.5-hour sessions every Tuesday & Thursday <br>for 4 weeks</em>
            </template>
          </b-card>
        </div>
        <div class="col-3">
          <b-card border-variant="light" header="Business Course" class="text-center h-100">
            <b-card-text><small>Intermediate</small></b-card-text>
            <b-card-text>
              <p>Dealing with Japanese clients most of the time? Impress them with your Japanese with this course.</p>
              <p>Learn how to speak and write formally in Japanese, the do's and dont's when dealing with Japanese clients and more.</p>
            </b-card-text>
            <template v-slot:footer>
                <em>Schedules may be flexible. <br>Please contact us for consultation.<br></em>
            </template>
          </b-card>
        </div>
        <div class="col-3">
          
          <b-card border-variant="light" header="JLPT Course" class="text-center h-100">
            <b-card-text><small>Beginner</small></b-card-text>
            <b-card-text>
                <p>Do you already have plans to go to work to Japan? Certification exams increase your chances of achieving those dreams.</p>
                <p>You will be taught Japanese in accordance to the strucutre of the JLPT Exams. Test yourself with mock tests that will be provided to assessyour Japanese.</p>
                <p>N5, N4, N5+N4, N3, N2</p>
                <p>Courses are available.</p>
              </b-card-text>
              <template v-slot:footer>
                <em>2-hour sessions every Tuesday & Thursday <br>for 12 weeks</em>
              </template>
          </b-card>
        </div>
      </div>



      <!-- <b-card-group deck class="mb-5 mx-5">
        <b-card border-variant="light" header="Tourist/Travel Course" class="text-center">
          <b-card-text>
            <p>Planning to visit Japan? Know Enough japanese to get around Jpaan and interact with the locals.</p>
            <p>You will be taught the basic writing conventions (Hiragana and Katakana) and useful expressions in Japanese. You willalso be given insights on the Japanese culture.</p>
            <hr />
            <p
              class="card-foo align-text-bottom"
            >2 -hour sessions every Wednesday & Friday for 4 weeks</p>
          </b-card-text>
        </b-card>
        <b-card border-variant="light" header="Hobbyist/Otaku Course" class="text-center mx-5">
          <b-card-text>
            <p>Do you admire Japan's culture? Or do you want to watch ani,e or manga without having to wait for subtitles? This course is for you.</p>
            <p>Conversational Japnese will be taught to you. Test your Japanese and immerse yourself by reading our wide ccollection of mangas and anime related materials.</p>
            <hr />
          </b-card-text>
          <div class="card-foo align-text-bottom">
            <p>1.5-hour sessions every Tuesday & Thursday for 4 weeks</p>
          </div>
        </b-card>
        <b-card border-variant="light" header="Business Course" class="text-center mx-5">
          <b-card-text>
            <p>Dealing with Japanese clients most of the time? Impress them with your Japanese with this course.</p>
            <p>Learn how to speak and write formally in Japanese, the do's and dont's when dealing with Japanese clients and more.</p>
            <hr>
          </b-card-text>
          <div class="card-foo position-relative">
            <p>Schedules may be flexible</p>
          </div>
        </b-card>
        <b-card border-variant="light" header="JLPT Course" class="text-center  mx-5">
          <b-card-text>
            <p>Do you already have plans to go to work to Japan? Certification exams increase your chances of achieving those dreams.</p>
            <p>You will be taught Japanese in accordance to the strucutre of the JLPT Exams. Test yourself with mock tests that will be provided to assessyour Japanese.</p>
            <p>N5, N4, N5+N4, N3, N2</p>
            <p>Courses are available.</p>
            <hr />
          </b-card-text>
          <div class="card-foo align-text-bottom">
            <p>2-hour sessions every Tuesday & Thursday for 12 weeks</p>
          </div>
        </b-card>
      </b-card-group> -->
    </div>
    <b-button type="button" class="btn btn-primary btn-lg p-3 my-5" variant="success">Get in touch with us</b-button>  
  </div>
</template>
<script>
</script>
<style scoped>
    .my-courses {
      height: 100vh;
    }

    div.card-header {
      font-size: 20px;
      font-weight: bolder;
      color: #54aa67;
    }
    div.card-body,
    div.card-header {
      background-color: #fffbe5;
    }
    .card-foo {
      font-weight: bolder;
      color: #54aa67;
      bottom: 0;
    }
    .btn-lg {
        font-size: 1.6rem;
    }
</style>
