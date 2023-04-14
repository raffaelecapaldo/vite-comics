<template>
 <div class="col-2">
    <div class="comic-card mt-3 me-3">
        <img class="cover" :src="image" :alt="title">
        <p class="text-white text-uppercase mt-3">{{ title }}</p>
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
</style>