<script>
export default {
    name: "FooterBluebar",
    data() {
        return {
            BarLinks: [
                {
                    title: "digital comics",
                    img: "buy-comics-digital-comics.png"
                },
                {
                    title: "dc merchandise",
                    img: "buy-comics-merchandise.png"
                },
                {
                    title: "subscription",
                    img: "buy-comics-subscriptions.png"
                },
                {
                    title: "comic shop locator",
                    img: "buy-comics-shop-locator.png"
                },
                {
                    title: "dc power visa",
                    img: "buy-dc-power-visa.svg"
                },
            ]
        }
    },
    methods: {
        getImagePath(img) {
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        }
    }

}
</script>

<template>
    <div id="main">
        <div class="container d-flex justify-content-between">
            <div class="d-flex align-items-center" id="linkCard" v-for="element in BarLinks">
                <img :src="getImagePath(element.img)" alt="">
                <a href=" #" class="text-white fw-semibold text-uppercase ms-3 text-decoration-none">{{
                    element.title
                }}</a>
            </div>
        </div>
    </div>
</template>
<style scoped>
#main {
    background-color: #0282f9;
}

#linkCard {
    height: 8rem;
}

img {
    height: 50%;
}
</style>