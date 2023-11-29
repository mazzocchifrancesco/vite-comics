<script>
export default {
    name: "FooterMain",
    data() {
        return {
            Card: [
                {
                    title: "dc comics",
                    links: ["characters", "comics", "movies", "TV", "games", "videos", "news"]
                },
                {
                    title: "shop",
                    links: ["shop DC", "shop DC collectibles"]
                },
                {
                    title: "dc",
                    links: ["term of use", "privacy policy (new)", "ad choices", "advertising", "jobs", "subscription", "talent workshops", "CPSC certificates", "ratings", "shop help", "contact us"]
                },
                {
                    title: "sites",
                    links: ["DC", "MAD magazine", "DC kids", "DC universe", "DC power visa"]
                },

            ]

        }
    },

}
</script>

<template>
    <div id="main">

        <div class="container d-flex justify-content-between">
            <div id="linkContainer" class=" d-flex flex-wrap flex-column gap-5">
                <div v-for="element in Card" class="d-flex flex-column">
                    <h3 class="text-uppercase text-white">{{ element.title }}</h3>
                    <a href="#" class="text-capitalize text-decoration-none text-secondary" v-for="link in element.links">
                        {{ link
                        }}</a>
                </div>
            </div>
            <div id="bgLogo"></div>
        </div>
    </div>
</template>
<style scoped>
#linkContainer {
    width: 35rem;
    height: 30rem;
    padding: 2rem 0;
}

#main {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;

}

#bgLogo {
    width: 50%;
    background-size: cover;
    background-position: center;
    background-image: url("../assets/img/dc-logo-bg.png");
}
</style>