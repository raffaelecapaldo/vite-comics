<template>
    <div class="comics">
  <div class="container">
    <div class="row pt-5">
  <ComicCard v-for="comic in comics" :image="comic.thumb" :title="comic.series" />
</div>
</div>
 </div>
</template>

<script>
import { comicsData } from '../data/data.js'
import ComicCard from './ComicCard.vue';
    export default {
        name:'comic-cards',
        components: {
            ComicCard,
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