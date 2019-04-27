<template>
  <div class="home">
    <header>
      <Navbar/>
      <div class="banner">
        <div class="header-content" >
          <h1 >
            體驗異國XXX的
          </h1>
          <p>
            為自己的身體請一天假。
          </p>
        </div>
      </div>
    </header>
    <main class="main-body" >
      <h2 class="mb-5">店內景觀</h2>
      <carousel :per-page="4" :navigate-to="someLocalProperty" :navigationEnabled="true" :paginationEnabled="false">
        <slide class="p-2 slide">
          <img src="../assets/image/slider1.jpg" alt="">
        </slide>
        <slide class="p-2 slide">
          <img src="../assets/image/slider2.jpg" alt="">
        </slide>
        <slide class="p-2 slide">
          <img src="../assets/image/slider3.jpg" alt="">
        </slide>
        <slide class="p-2 slide">
          <img src="../assets/image/slider4.jpg" alt="">
        </slide>
        <slide class="p-2 slide">
          <img src="../assets/image/slider5.jpg" alt="">
        </slide>
        <slide class="p-2 slide">
          <img src="../assets/image/slider6.jpg" alt="">
        </slide>
        <slide class="p-2 slide">
          <img src="../assets/image/slider7.jpg" alt="">
        </slide>
        <!-- <slide class="col-3">
          <img src="../assets/image/slider8.jpg" alt="">
        </slide> -->
      </carousel>
    </main>
    <article>
      <h2 class="mb-5">陶板浴介紹</h2>
        <div class="article-content container">
          <div class="row">
          <div class="col-6">
            <img src="../assets/image/ofuro_ganbanyoku.png" alt="">
          </div>
          <div class="col-6">
            <h4>陶板浴簡介</h4>
            <p>
              汗水從體內深層緩慢釋出到20分鐘左右快速流汗從皮脂腺代謝體內毒素等。因細胞活化所排出汗水如同天然的化妝水皮脂膜可以保護肌膚快速衝掃或擦拭身體即可無須沐浴乳。
              從體內深層持續緩和的讓平時體溫上升改善手腳冰冷體質。
              活性氣類減少腦波轉α波幫助入眠。
              病原菌會被除去，腸內益菌會增加
              身體內部新陳代謝加速且流汗量少時體內毒素由排尿釋出。
              乳酸被分解痛去除。
            </p>
          </div>
          <div class="col-6"></div>
          <div class="col-6"></div>
        </div>
      </div>
    </article>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue'
import { Carousel, Slide } from 'vue-carousel'

export default {
  name: 'home',
  components: {
    Navbar,
    Carousel,
    Slide
  }
}
</script>
<style scoped lang="scss">
header {
  height: 100vh;
  background-image: url('../assets/image/bg2.jpg');
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;

  .banner {
    height: 100%;
    display:flex;
    align-items:center;
    justify-content:center;
  }

  .header-content {
    margin: auto;
    height: 60%;
    width: 60%;
    background-color: rgba(0, 0, 0, 0.3);
    color: #fff;
    padding: 80px;
  }
}
.main-body {
  width: 90%;
  margin: 5%;
}
img {
  width: 100%;
  height: 100%;
}

</style>
<style>
  .VueCarousel-navigation-button {
    font-size: 3rem;
    color: #fff !important;
  }
</style>
