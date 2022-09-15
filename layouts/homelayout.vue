<template>
    <div class="home-layout">
        <HeaderMobile  />
        <Nuxt  />
        <FooterMobile  />
    </div>
</template>
<script>
    import FooterMobile from "~/components/FooterMobile.vue"
    import HeaderMobile from "~/components/HeaderMobile.vue"

export default {
    name: "homelayout",
    components: {
        FooterMobile,
        HeaderMobile
    }
}
</script>
<style></style>