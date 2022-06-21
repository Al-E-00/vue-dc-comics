<template>
    <div>
        <div class="row bg-primary">
            <div v-for="(link, i) in navLinks" :key="i" class="col">
                <img :src="require(`${link.img}`)" :alt="link.src">
                <p>{{ link.text }}</p>
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
                    img:"../src/assets/img/buy-comics-digital-comics.png",
                    src:"DC Digital Comics",
                    text:"Digital Comics"
                },
                {
                    img:"../../src/assets/img/buy-comics-merchandise.png",
                    src:"DC Merchandise",
                    text:"DC Merchandise"
                },
                {
                    img:"../../src/assets/img/buy-comics-subscriptions.png",
                    src:"DC Subscription",
                    text:"Subscription"
                },
                {
                    img:"../../src/assets/img/dc-logo-bg.png",
                    src:"DC Shop Locator",
                    text:"Comic Shop Locator"
                },
                {
                    img:"../../src/assets/img/buy-dc-power-visa.svg",
                    src:"DC Visa",
                    text:"Dc Power Visa"
                },
            ]
        }
    }
}
</script>

<style>
@import "../assets/scss/SectionNavigation.scss";
</style>