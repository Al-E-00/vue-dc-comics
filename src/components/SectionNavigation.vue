<template>
    <div>
        <div class="container-fluid">
            <div class="row bg-primary custom-navlinks-section gap-4">
                <div v-for="(link, i) in navLinks" :key="i" class="col d-flex align-items-center">
                    <img class="img-custom-navlinks" :src='require("../assets/" + link.img)' alt="img">
                    <p class="m-0 text-white">{{ link.text.toUpperCase() }}</p>
                </div>
            </div>

        </div>
    </div>
</template>

<script>
export default {
    name:"SectionNavigation",
    data() {
        return {
            navLinks: [
                {
                    img:"img_nav_banner_blu/buy-comics-digital-comics.png",
                    src:"DC Digital Comics",
                    text:"Digital Comics"
                },
                {
                    img:"img_nav_banner_blu/buy-comics-merchandise.png",
                    src:"DC Merchandise",
                    text:"DC Merchandise"
                },
                {
                    img:"img_nav_banner_blu/buy-comics-subscriptions.png",
                    src:"DC Subscription",
                    text:"Subscription"
                },
                {
                    img:"img_nav_banner_blu/buy-comics-shop-locator.png",
                    src:"DC Shop Locator",
                    text:"Comic Shop Locator"
                },
                {
                    img:"img_nav_banner_blu/buy-dc-power-visa.svg",
                    src:"DC Visa",
                    text:"Dc Power Visa"
                },
            ]
        }
    }
}
</script>

<style lang="scss">
@import "../assets/scss/SectionNavigation.scss";
</style>