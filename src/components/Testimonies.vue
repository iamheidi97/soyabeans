/* eslint-disable vue/no-unused-components */
<template>
  <div class="my-testimonies">
    <!-- <Sakura/> -->
    <h1 class="font-weight-bolder my-5 green-text mx-4">What some of our students had to say</h1>

    <div class="row justify-content-center mt-5">

      <div class="col-xl-4 col-lg-6 col-sm-12">
        <b-card img-src img-alt="Image" img-top class="h-100">
          <b-card-text class="px-4">
            <img
              src="../assets/images/Testimonials/Hannah-san.png"
              class="img-fluid rounded-pill up my-3"
            />
            <p
              class="justify-center font-italic"
            >I am currently living in Japan right now and whether you believe it or not, it is very difficult to communicate with Japanese if you don't have knowledge about Nihonggo. Before I went to Japan, my fiance before who is my husband right now already warned me about the possible difficulties I will be facing when I live there, and the most difficult is of course on how I can communicate with Japanese. I am so happy that I was able to learn Japanese first before I came to Japan. I learned the best knowledge, in the best way from the best teacher in Soya Beans. And now, I am not scared to talk with the sales lady on the counter here in their department stores nor scared to find jobs because I know how to communicate with them and I love it. 🥰 Thanks Soya Beans and to my beloved teacher Tomoko sensei 😻!</p>
          </b-card-text>
          <template v-slot:footer>
            <footer class="blockquote-footer bigger-text font-weight-bold">Hanah Radaza-Sato <br>🌸 ハナさん</footer>
          </template>
        </b-card>
      </div>
      <div class="col-xl-4 col-lg-6 col-sm-12">
        <b-card img-src img-alt="Image" img-top class="h-100">
          <b-card-text class="px-4">
            <img
              src="../assets/images/Testimonials/Allenjen-san.png"
              class="img-fluid rounded-pill up my-3"
            />
            <p
              class="justify-center"
            >原先生から学んだ事が日本で生活する上で、大いに役に立ちました。非常に感謝しています。原先生だけでなくSoya Beans Japanese Language School の他のスタッフの方々にとても感謝しています。</p>
            <p
              class="justify-center font-italic"
            >As a newbie here in Japan, everything excites me. From riding a train to exploring around, from enjoying spring and fall to conquering summer and winter. Despite this amazing experience, my life here is not as smooth as what everyone thinks. Aside from the fact that I’m away from home, I have to deal with drastic changes and pressures in studying while working. Everyday is a new day to challenge myself but I always do my best to manage everything. With God’s help, I am able to maintain my grades and excel in our class. In fact , recently I was able to pass JLPT N3 in less than a year of studying here . The determination I have, the prayers and help from my mentors lead me to where I am right now. </p><p class="justify-center">今後更に勉強して、N2 を目指します。</p>
          </b-card-text>
          <template v-slot:footer>
            <footer class="blockquote-footer bigger-text font-weight-bold">Allenjen Ursabia<br>✨ アレンジェンさん</footer>
      
          </template>
        </b-card>
      </div>
      
    </div>
    <div class="row mt-5">
      <p class="col-6"></p>
          <h2 class="green-text container text-center">特定技能介護日本語試験</h2>
          <h2 class="green-text container">合格おめでとう！</h2>
          <h4 class="green-text container font-weight-bold">Congratulations to our students <br>who passed the Nursing Care Japanese Language Evaluation Test!</h4>
    </div>
    <div class="row justify-content-center mt-3">
        <div class="col-xl-4 col-lg-6 col-sm-12">
        <b-card img-src img-alt="Image" img-top class="h-100">
          <b-card-text class="px-4">
            <img
              src="../assets/images/Testimonials/p1.jpeg"
              class="img-fluid rounded-pill down my-3"
            />
            <p
              class="justify-center font-italic"
            >We thoroughly enjoyed our Japanese Style Caregiving lessons in 2 months with Sensei Hara. She is fun, encouraging and always prepared. She able to make us feel comfortable and welcome.</p>
            <p class="justify-center font-italic">
              We learned a lot about the basic knowledge of Caregiving (Kaigo) in 2 months. Although It is difficult to memorize the Chinese characters and nursing care terminology. We did to passed the 2 exam the nursing care skill evaluation test and nursing care japanese language evaluation test.
              Of course its because of our beloved teachers and staff. It is because of them were now successful for applying Japan as care worker.
              </p>
              <p>いろいろお世話になりました。</p>
            <p class="justify-center font-italic">
              💯💯
              We highly recommend this class for anyone interested in Japanese Style Caregiving lessons or as a supplement class to improve their Japanese Language Proficiency and also applying Japan as care worker.
            </p>
          </b-card-text>
          <template v-slot:footer>
            <footer class="blockquote-footer bigger-text font-weight-bolder">Anna, Chai, Jonas <br> 👨‍👩‍👧 アナさん、チャイさん、ジョナスさん</footer>
          </template>
        </b-card>
      </div>
    </div>
  </div>
</template>

<script>

</script>

<style scoped>
    @media (max-width: 576px) {
      h1 {
        font-size: 2rem;
      }
    }
    .down {
      width: 12em !important;
    }
    .up {
      width: 10em !important;
    }
    .justify-center {
      text-align: justify;
      text-align-last: center;
      font-size: 0.9em;
    }
    .bigger-text {
      font-size: 1.1em;
    }
    .my-testimonies {
      margin-top: 10em;
      margin-bottom: 10em;
    }
    .card {
      border: none;
    }
    .card-footer {
      background-color: rgba(0, 0, 0, 0);
      border-top: none;
    }
    .blockquote-footer {
      color: #158c39;
    }
</style>