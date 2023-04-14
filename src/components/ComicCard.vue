<template>
 <div class="col-xxl-2 col5 col-lg-3 col-md-4 col-sm-6 col-6  d-flex d-sm-block justify-content-center align-items-center">
    <div class="comic-card mt-3 d-flex flex-column justify-content-center align-items-center d-sm-block">
        <img class="cover" :src="image" :alt="title">
        <div class="text-cover">
        <p class="text-white text-uppercase mt-3 ">{{ title }}</p>
        </div>
    </div>
 </div>   
</template>

<script>
    export default {
    name:"comic-card",
    props: ['image', 'title'],
    data() {
        return {

        }
    }
        
    }
</script>

<style lang="scss" scoped>
.cover {
    width: 187px;
    height: 187px;
}

@media (max-width: 1400px) and (min-width:1199.98px) {.col5 {
    flex: 0 0 auto;
    width: 20%;
}}
</style>