<script>
import mainGame from './mainGame.vue'
import AppGaming from './AppGamingArea.vue'
import AppStreaming from './AppStreamingArea.vue'
import AppBattle from './AppBattle.vue'
import AppTreading from './AppTreading.vue'
import AppMatch from './AppMatch.vue'
import AppTeam from './AppTeam.vue'
import AppTestimonial from './AppTestimonial.vue'
import AppShop from './AppShop.vue'
import AppNews from './AppNews.vue'

export default {
  name: 'AppMain',
  components:{
    mainGame,
    AppGaming,
    AppStreaming,
    AppBattle,
    AppTreading,
    AppMatch,
    AppTeam,
    AppTestimonial,
    AppShop,
    AppNews,
  },
  data() {
    return {
      imageUrls: [
        './src/assets/img/1.png',
        './src/assets/img/2.png',
        './src/assets/img/3.png',
        './src/assets/img/4.png',
        './src/assets/img/5.png',
        './src/assets/img/6.png'
      ]
    };
  },
  mounted() {
    console.log(this.imageUrls);
  }
}
</script>

<template>
    <section class="ms-bg-section">
        <div class="container position-relative">
            <div class="box-img">
                <img v-for="(imageUrl, index) in imageUrls" :key="index" :src="imageUrl" alt="" class="mx-4 py-3 px-2">
            </div>
            
        </div>
        <mainGame></mainGame>    
    </section>
    <section id="gaming-area">
          <AppGaming></AppGaming>
    </section>
    <section id="streaming-area">
      <AppStreaming></AppStreaming>
    </section>
    <section id="battle-area">
      <AppBattle></AppBattle>
    </section>
    <section id="treading-area">
      <AppTreading></AppTreading>
    </section>
    <section id="match-area">
      <AppMatch></AppMatch>
    </section>
    <section id="team-area">
        <AppTeam></AppTeam>
    </section>
    <section id="testimonial-area">
      <AppTestimonial></AppTestimonial>
    </section>
    <section id="shop-area">
      <AppShop></AppShop>
    </section>
    <section id="news-area">
      <AppNews></AppNews>
    </section>

</template>

<style scoped>
 .ms-bg-section {
    background-color: #191935;
    height: 40vw;
    color: white;
 }


 .box-img {
    background-color: #202046;
    height: 200px;
    width: 1230px;
    position: absolute;
    bottom: -100px;
    left: 40px;
 }
</style>