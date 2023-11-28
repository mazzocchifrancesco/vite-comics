<script>
import FooterBluebar from '../components/FooterBluebar.vue'
import FooterMain from '../components/FooterMain.vue'
import FooterSocials from '../components/FooterSocials.vue'


export default {
    name: "AppFooter",
    components: {
        FooterBluebar,
        FooterMain,
        FooterSocials
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
    <FooterSocials />
</template>

<style scoped></style>