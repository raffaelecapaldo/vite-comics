<template>
    <nav>
        <div class="container d-flex justify-content-between text-white p-3">
            <div class="links w-50 d-flex justify-content-between">
                <div v-for="group in groupLinks" class="group-link">
                    <h3 class="fw-bold fs-5 text-uppercase">{{group.title}}</h3>
                    <ul>
                       <a class="small" v-for="link in group.links" href=""> <li>{{ link.text }}</li></a>
                    </ul>
                </div>
            </div>
            <div class="bg-footer">
                <img src="img/dc-logo-bg.png" alt="">
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
    background-image: url('img/footer-bg.jpg');

    background-repeat: no-repeat;
    background-size: cover;
}


nav {
    ul {
        list-style: none;
        padding:0;
        margin:0;

        a {
        color:#71776e;
        text-decoration:none;
        }
    }

}
.bg-footer {
    position:relative;
    img {
        position:absolute;
        right:0;
        top:-80px;
    }
}

</style>