<template>
 <AppHeader />
 <Jumbotron />
 <main>
 <ComicCards />
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
import Jumbotron from './components/Jumbotron.vue';
import ComicCards from './components/ComicCards.vue';

  export default {
   components: {
    AppHeader,
    DCItems,
    FooterNav,
    FooterBottom,
    Jumbotron,
    ComicCards
   },
  }
</script>

<style lang="scss" scoped>

</style>