<template>
    <footer dir="rtl" class="fixed bottom-0 w-full h-16
    flex justify-evenly items-center text-3xl shadow-2xl">
        <nuxt-link to="/home" id="home-nav-el">
            <i class="el-icon-house"></i>
        </nuxt-link>
        <nuxt-link to="/calendar" id="calendar-nav-el">
            <i class="el-icon-date"></i>
        </nuxt-link>
        <nuxt-link to="/shopping" id="shopping-nav-el">
            <i class="el-icon-shopping-bag-2"></i>
        </nuxt-link>
        <nuxt-link to="/phone" id="phone-nav-el">
            <i class="el-icon-phone-outline"></i>
        </nuxt-link>
        <nuxt-link to="/favourites" id="fav-nav-el">
            <i class="el-icon-star-off"></i>
        </nuxt-link>
    </footer>
</template>
<script>

export default {
    name: 'FooterMobile'
}
</script>
<style scoped>
footer {
    background-color: #dfd8d8;
}
#shopping-nav-el {
    transform: translateY(-0.8em);
    background:  linear-gradient(145deg, #c8c8c8, #eeeeee);
    box-shadow:  5px 5px 10px #bdbdbd,
             -5px -5px 10px #ffffff;
    border-radius: 10rem;
    padding: 0.8rem;
    display: grid;
    place-items: center;
}
.nuxt-link-exact-active > i {
    color: green;
    transition: color 200ms;
}
</style>