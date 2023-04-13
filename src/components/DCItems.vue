<template>
    <div class="items-dc">
        <div class="container p-5">
            <div class="d-flex justify-content-around align-items-center">
                <div v-for="item in items" class="item text-white">
                    <img :class="{small: item.text === 'Comic Shop Locator'}" :src="item.image" alt="">
                    <span class="ms-3 text-uppercase">{{ item.text }}</span>
                </div>
              
            </div>
        </div>
    </div>
</template>

<script>
import { items } from '../data/data.js'

    export default {
        name:"dc-items",
        data() {
            return {
               items:items 
            }
        }
    }
</script>

<style lang="scss" scoped>
.items-dc {
    background-color: #0282f9;
}

.item {
    img {
        width:55px;
    }
}

.small {
    width:40px !important;
}
</style>