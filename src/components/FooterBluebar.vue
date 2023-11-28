<script>
export default {
    name: "FooterBluebar",
    data() {
        return {
            BarLinks: [
                {
                    title: "digital comics",
                    img: "../src/assets/img/buy-comics-digital-comics.png"
                },
                {
                    title: "dc merchandise",
                    img: "../src/assets/img/buy-comics-merchandise.png"
                },
                {
                    title: "subscription",
                    img: "../src/assets/img/buy-comics-subscription.png"
                },
                {
                    title: "comic shop locator",
                    img: "../src/assets/img/buy-comics-shop-locator.png"
                },
                {
                    title: "dc power visa",
                    img: "../src/assets/img/buy-dc-power-visa.svg"
                },
            ]
        }
    },

}
</script>

<template>
    <div id="main">
        <div class="container d-flex justify-content-between">
            <div class="d-flex align-items-center" id="linkCard" v-for="element in BarLinks">
                <img :src="element.img" alt="">
                <p class="text-white fw-semibold text-uppercase ms-3">{{ element.title }}</p>
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