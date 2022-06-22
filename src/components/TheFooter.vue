<template>
    <div>
        <div class="container-fluid">
            <div class="row background-the-footer">
                <div class="background-the-footer-second-layer"></div>
                <div class="col-2">
                    <ul>
                        <h3 class="text-uppercase">Dc Comics</h3>
                        <li v-for="(name, i) in dcComics" :key="i">
                            <a href="#">{{ name.name }}</a>
                        </li>
                    </ul>
                    <ul>
                        <h3 class="text-uppercase">Shop</h3>
                        <li v-for="(name, i) in shop" :key="i">
                            <a href="#">{{ name.name }}</a>
                        </li>
                    </ul>
                </div>
                <div class="col-2">
                    <ul>
                        <h3 class="text-uppercase">Dc</h3>
                        <li v-for="(name, i) in DC" :key="i">
                            <a href="#">{{ name.name }}</a>
                        </li>
                    </ul>
                </div>
                <div class="col-2">
                    <ul>
                        <h3 class="text-uppercase">Sites</h3>
                        <li v-for="(name, i) in Sites" :key="i">
                            <a href="#">{{ name.name }}</a>
                        </li>
                    </ul>
                </div>
        </div>
    </div>
    </div>
</template>

<script>
export default {
    name: "TheFooter",
    data() {
        return {
            dcComics: [
                {
                    name: "Characters",
                },
                {
                    name: "Comics",
                },
                {
                    name: "Movies",
                },
                {
                    name: "TV",
                },
                {
                    name: "Games",
                },
                {
                    name: "Videos",
                },
                {
                    name: "News",
                },
            ],
            shop: [
                {
                    name: "Shop DC",
                },
                {
                    name: "Shop DC Collectibles",
                },
            ],
            DC: [
                {
                    name: "Terms Of Use"
                },
                {
                    name: "Privacy policy (New)"
                },
                {
                    name: "Ad Choices"
                },
                {
                    name: "Advertising"
                },
                {
                    name: "Jobs"
                },
                {
                    name: "Subscriptions"
                },
                {
                    name: "Talent Workshops"
                },
                {
                    name: "CPSC Certificates"
                },
                {
                    name: "Ratings"
                },
                {
                    name: "Shop Help"
                },
                {
                    name: "Contact Us"
                },
            ],
            Sites: [
                {
                    name: "DC"
                },
                {
                    name: "MAD Magazine"
                },
                {
                    name: "DC Kids"
                },
                {
                    name: "DC Universe"
                },
                {
                    name: "DC Power Visa"
                }
            ]
        }
    }
}

</script>

<style lang="scss">
@import "../assets/scss/FooterStyles.scss"
</style>