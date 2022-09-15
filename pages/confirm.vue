<template>
    <div class="h-full w-full flex justify-center">
        <LoginConfirmCard  />
    </div>
</template>

<script>
    import LoginConfirmCard from "~/components/LoginConfirmCard.vue"

    export default {
        name: 'confirm',
        layout: 'mobileloginlayout',
        components: {
            LoginConfirmCard
        }
    }
</script>

<style></style>