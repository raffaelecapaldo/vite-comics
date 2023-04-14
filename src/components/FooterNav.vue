<template>
    <nav>
        <div class="container d-flex justify-content-between text-white pt-5">
            <div class="links d-flex justify-content-between flex-wrap flex-sm-nowrap">
                <div v-for="group in groupLinks" class="group-link">
                    <h3 class="fw-bold fs-5 text-uppercase">{{group.title}}</h3>
                    <ul>
                       <a class="small" v-for="link in group.links" :href="link.url"> <li>{{ link.text }}</li></a>
                    </ul>
                </div>
            </div>
            <div class="bg-footer d-none d-lg-block">
                <img src="/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </nav>
</template>

<script>
import { footerLinks } from '../data/data.js'

    export default {
        name:'footer-nav',
        data() {
            return {
                groupLinks:footerLinks
            }
        }
        
    }
</script>

<style lang="scss" scoped>

nav {
    background-image: url('/img/footer-bg.jpg');

    background-repeat: no-repeat;
    background-size: cover;
}

.links {
    width: 50%;
}

.container {
    height: 450px;
}

nav {
    ul {
        list-style: none;
        padding:0;
        margin:0;

        a {
        color:#71776e;
        text-decoration:none;

        &:hover{
            color:#0282f9;
        }
        }
    }

}
.bg-footer {
    overflow: hidden;
 img {
    width:563px;
    overflow: hidden;
    object-position: 0 -76px;
 }
}

@media screen and (max-width:992px) {
    .links {
        width:100%;
    }
}

</style>