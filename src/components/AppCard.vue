<script>
export default {
    props:
        ["products"]
}
</script>

<template>
    <div class="row">
        <div class="col-2" id="card" v-for="prodotto in products">
            <img :src="prodotto.thumb" alt="">
            <p class="text-uppercase">{{ prodotto.series }}</p>
        </div>
    </div>
</template>

<style scoped>
img {
    width: 100%;
    aspect-ratio: 1;
    margin-bottom: 1rem;
}

#card {}
</style>