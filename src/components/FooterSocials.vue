<script>
export default {
    name: "FooterSocials",
    data() {
        return {
        }
    },

}
</script>
<template>
    <div id="main" class="d-flex align-items-center">
        <div class="container d-flex justify-content-between">
            <div id="signUp" class="text-uppercase text-white p-2 d-inline-block fw-semibold">
                sign-up now!
            </div>
            <div class="d-flex gap-3 align-items-center">
                <div class="text-uppercase fw-bold text-primary">follow us</div>
                <i class="fa-brands fa-facebook-f rounded-circle"></i>
                <i class="fa-brands fa-twitter rounded-circle"></i>
                <i class="fa-brands fa-youtube rounded-circle"></i>
                <i class="fa-brands fa-pinterest-p rounded-circle"></i>
                <i class="fa-solid fa-location-dot rounded-circle"></i>

            </div>
        </div>
    </div>
</template>
<style scoped>
#main {
    background-color: #303030;
    height: 6rem;
}

#signUp {
    border: solid 2px #008bff;
}

i {
    background-color: #797979;
    height: 2rem;
    aspect-ratio: 1;
    display: flex;
    align-items: center;
    justify-content: center;
}
</style>