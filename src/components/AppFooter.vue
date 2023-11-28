<script>
import FooterBluebar from '../components/FooterBluebar.vue'
import FooterMain from '../components/FooterMain.vue'

export default {
    name: "AppFooter",
    components: {
        FooterBluebar,
        FooterMain
    },
    data() {
        return {

        }
    },

}
</script>

<template>
    <FooterBluebar />
    <FooterMain />
</template>

<style scoped></style>