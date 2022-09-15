<template>
    <div class="home-content pt-28">
        <HomeContentComponent  />
    </div>
</template>

<script>
import HomeContentComponent from "~/components/HomeContentComponent.vue"

export default {
    name: 'home',
    layout: 'homelayout',
    components: {
        HomeContentComponent
    }
}
</script>
<style>

</style>