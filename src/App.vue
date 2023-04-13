<template>
 <AppHeader />
 <main>
 <div class="todo fs-3 bg-black p-5 text-white">
  <div class="container">
    Content Goes Here
  </div>
 </div>
 <DCItems />
 <footer>
 <FooterNav />
</footer>


 </main>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import DCItems from './components/DCItems.vue';
import FooterNav from './components/FooterNav.vue';
  export default {
   components: {
    AppHeader,
    DCItems,
    FooterNav
   } 
  }
</script>

<style lang="scss" scoped>

</style>