<template>
    <div class="items-dc">
        <div class="container p-5">
            <div class="d-flex justify-content-around align-items-center flex-wrap gap-3">
               <DCItem v-for="item in items" :text="item.text" :image="item.image"/>            
            </div>
        </div>
    </div>
</template>

<script>
import { items } from '../data/data.js'
import DCItem from './DCItem.vue';
    export default {
        name:"dc-items",
        data() {
            return {
               items:items 
            }
        },
        components: {
            DCItem
        }
    }
</script>

<style lang="scss" scoped>
.items-dc {
    background-color: $primary-color;
}
</style>