<template>
 <AppHeader />
 <Jumbotron />
 <main>
 <div class="comics">
  <div class="container">
    <div class="row">
  <ComicCard v-for="comic in comics" :image="comic.thumb" :title="comic.series" />
</div>
</div>
 </div>
 <DCItems />
 <footer>
 <FooterNav />
 <FooterBottom />
</footer>


 </main>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import DCItems from './components/DCItems.vue';
import FooterNav from './components/FooterNav.vue';
import FooterBottom from './components/FooterBottom.vue';
import ComicCard from './components/ComicCard.vue';
import Jumbotron from './components/Jumbotron.vue';
import { comicsData } from './data/data.js'

  export default {
   components: {
    AppHeader,
    DCItems,
    FooterNav,
    FooterBottom,
    ComicCard,
    Jumbotron,
   },
   data() {
    return {
      comics: comicsData
    }
   } 
  }
</script>

<style lang="scss" scoped>
.comics {

  background-color: #1c1c1c;
}
</style>