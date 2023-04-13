<template>
 <div class="footer-bottom">
    <div class="container d-flex justify-content-between align-items-center">
        <div class="call-to-action">
            <a class="text-uppercase" href="#">sign-up now!</a>
        </div>
        <div class="social d-flex align-items-center">
            <span>Follow Us</span>
            <img src="img/footer-facebook.png" alt="facebook">
            <img src="img/footer-twitter.png" alt="twitter">
            <img src="img/footer-youtube.png" alt="youtube">
            <img src="img/footer-pinterest.png" alt="pinterest">
            <img src="img/footer-periscope.png" alt="periscope">

        </div>
    </div>
 </div>   
</template>

<script>
    export default {
        name:'footer-bottom',
        
    }
</script>

<style lang="scss" scoped>
.footer-bottom {
    background-color: #303030;
}

.call-to-action {
    a {
        color:white;
        text-decoration: none;
        border:2px solid #0282f9;
        padding:15px;
        font-weight: bold;
    }
}

.container {
    padding:50px;
}

.social {
    img {
        margin-left:1rem;
    }
    span {
        color: #0282f9;
        text-transform: uppercase;
        font-size: 1.5rem;
        font-weight: bold;
    }
}
</style>