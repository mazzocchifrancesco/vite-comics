<script>
export default {
    name: "AppHeader",
    data() {
        return {
            menuLinks: [
                {
                    text: "CHARACTERS",
                    url: "#CHARACTERS",
                },
                {
                    text: "COMICS",
                    url: "#COMICS",
                },
                {
                    text: "MOVIES",
                    url: "#MOVIES",
                },
                {
                    text: "TV",
                    url: "#TV",
                },
                {
                    text: "GAMES",
                    url: "#GAMES",
                },
                {
                    text: "COLLECTIBLES",
                    url: "#COLLECTIBLES",
                },
                {
                    text: "VIDEOS",
                    url: "#VIDEOS",
                },
                {
                    text: "FANS",
                    url: "#FANS",
                },
                {
                    text: "NEWS",
                    url: "#NEWS",
                },
                {
                    text: "SHOP",
                    url: "#SHOP",
                },
            ]
        }
    },

}
</script>

<template>
    <header>
        <div class="container d-flex justify-content-between">

            <img src="../assets/img/dc-logo.png" alt="">
            <nav class="d-flex gap-3 align-items-center">
                <a class="text-decoration-none text-secondary fw-bold" v-for="link in menuLinks" :href="link.url">{{
                    link.text
                }}</a>
            </nav>
        </div>
    </header>
</template>

<style scoped>
img {
    height: 5rem;
    margin: 1rem 0;
}
</style>