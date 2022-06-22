<template>
    <div>
        <div class="container-fluid">
            <div class="row bg-secondary custom-style-banner">

                <div class="col ">
                    <button class="btn btn-outline-primary text-uppercase button-custom-style">Sign Up Now!</button>
                </div>
                <div class="col d-flex justify-content-end align-items-center gap-3 custom-style-link-banner">
                    <a class="text-uppercase" href="#">Follow us</a>
                    <img src="img/footer-facebook.png" alt="">
                    <img src="img/footer-twitter.png" alt="">
                    <img src="img/footer-youtube.png" alt="">
                    <img src="img/footer-pinterest.png" alt="">
                    <img src="img/footer-periscope.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
name:"BannerSignUp",
}
</script>

<style lang="scss" >
    @import "../assets/scss/BannerSignUp.scss";
</style>