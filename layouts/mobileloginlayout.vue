<!-- login layout  -->
<template>
    <div class="layout w-screen h-screen lg:hidden" >
        <img src="~/assets/images/5xjA4S.png" alt="fit body">
        <Nuxt  />
    </div>
</template>
<script>

    export default {
        name: 'mobileloginlayout'
    }
</script>
<style scoped>
img {
    object-fit: cover;
    width: 100%;
    height:100%;
    position: absolute;
    z-index: -1;
    object-position: 33% 0 ;
}
</style>