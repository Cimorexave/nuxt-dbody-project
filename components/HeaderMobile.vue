<template>
    <header dir="rtl" class="fixed bg-white z-10 p-3 px-5 gap-3 pb-1 top-0 right-0 w-full h-max flex flex-col justify-between">
        <div class="flex justify-between items-center">
            <img src="~/assets/images/menu.png" alt="menu icon">
            <img src="~/assets/images/Group.png" class="scale-75" alt="app logo">
            <i class="el-icon-bell text-lg"></i>
        </div>
        <div class="user-info flex justify-between text-green-500 text-sm">
            <p class="font-bold">
                مهرداد مظفری
            </p>
            <p class="font-light">
                امتیاز شما: 10
            </p>
        </div>
    </header>
</template>
<script>

export default {
    name: 'HeaderMobile'
}
</script>
<style>
    
</style>