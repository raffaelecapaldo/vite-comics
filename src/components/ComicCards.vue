<template>
    <div class="comics">
     
  <div class="container">
    <div class="showtitle text-white fs-3 fw-bold text-uppercase">
            current series 
        </div>
    <div class="row pt-5">
  <ComicCard v-for="comic in comics" :image="comic.thumb" :title="comic.series" />
</div>
<div class="load text-white d-flex justify-content-center text-uppercase">
    <span>load more</span>
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
.container {
    span {
        background-color: $primary-color;
        padding:10px 50px;
        margin-top:35px;
        margin-bottom:20px;
        font-weight: bold;
        cursor:pointer;
    }
    position:relative

}
.showtitle {
    position: absolute;
    top:-40px;
    left:-5px;
    background-color: $primary-color;
    padding:10px 18px;
}
}
</style>