<template>
    <div>
        <div class="d-flex justify-content-between custom-nav-style">
            <img class="logo-image-navbar" src="img/dc-logo.png" alt="Logo DC">
            <ul class="d-flex gap-4 m-0 list-unstyled align-items-center">
                <li v-for="(links, i) in navLinks" :key="i" >
                    <a class="links-navbar " :href="links.href" :class="links.isActive ? 'active' : ''" @click="changeActive(i)">{{ links.name.toUpperCase() }}</a>
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
                    isActive: false,
                },
                {
                    name: "comics",
                    href: "#",
                    isActive: true
                },
                {
                    name: "movies",
                    href: "#",
                    isActive: false
                },
                {
                    name: "tv",
                    href: "#",
                    isActive: false
                },
                {
                    name: "games",
                    href: "#",
                    isActive: false
                },
                {
                    name: "collectibles",
                    href: "#",
                    isActive: false
                },
                {
                    name: "videos",
                    href: "#",
                    isActive: false
                },
                {
                    name: "fans",
                    href: "#",
                    isActive: false
                },
                {
                    name: "news",
                    href: "#",
                    isActive: false
                },
                {
                    name: "shop",
                    href: "#",
                    isActive: false
                }
            ]
        }
    },
    methods: {
        changeActive(i) {
            if(this.navLinks[i].isActive === true) {
                return
            } else {
                for (let i = 0; i < this.navLinks.length; i++) {
                    this.navLinks[i].isActive = false;
                }
                this.navLinks[i].isActive = true;
            }
        }
    }
}
</script>

<style lang="scss">
@import "../assets/scss/HeaderStyles.scss";

</style>