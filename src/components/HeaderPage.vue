<template>
    <div>
        <div class="d-flex justify-content-between custom-nav-style">
            <img class="logo-image-navbar" src="../assets/img/dc-logo.png" alt="Logo DC">
            <ul class="d-flex gap-4 m-0 list-unstyled align-items-center">
                <li v-for="(links, i) in navLinks" :key="i">
                    <a class="links-navbar text-dark" :href="links.href">{{ links.name.toUpperCase() }}</a>
                </li>
            </ul>

        </div>
    </div>
</template>

<script>
export default {
    name: "TheHeader",
    data() {
        return {
            navLinks: [
                {
                    name: "characteristic",
                    href: "#",
                },
                {
                    name: "comics",
                    href: "#",
                },
                {
                    name: "movies",
                    href: "#",
                },
                {
                    name: "tv",
                    href: "#",
                },
                {
                    name: "games",
                    href: "#",
                },
                {
                    name: "collectibles",
                    href: "#",
                },
                {
                    name: "videos",
                    href: "#",
                },
                {
                    name: "fans",
                    href: "#",
                },
                {
                    name: "news",
                    href: "#",
                },
                {
                    name: "shop",
                    href: "#",
                }
            ]
        }
    }
}
</script>

<style lang="scss">
@import "../assets/scss/HeaderStyles.scss";

</style>