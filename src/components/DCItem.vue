<template>
    <div class="item text-white">
        <img :class="{ small: text === 'Comic Shop Locator' }" :src="image" :alt="text">
        <span class="ms-3 text-uppercase">{{ text }}</span>
    </div>
</template>

<script>
export default {
    name:'dc-item',
    props: ['text', 'image']

}
</script>

<style lang="scss" scoped>
.item {
    img {
        width:55px;
    }
}

.small {
    width:40px !important;
}
</style>
