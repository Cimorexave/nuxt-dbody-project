<template>
    <LoginComponentMobile  />
</template>
<script>
import LoginComponentMobileVue from '~/components/LoginComponentMobile.vue';

export default {
        name: "login",
        layout: 'mobileloginlayout',
        components: {
            LoginComponentMobileVue
        }
    }
</script>
<style scoped>

</style>