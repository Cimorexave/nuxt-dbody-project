<!-- This is the error page. although it's in the layouts directory 
but it is basically rendered as a page, this page will show in res.status: 404, 500,...  -->
<template>
    <div dir="rtl" class="grid place-items-center h-screen">
        <div class="error-content">
            <h1 class="text-xl font-bold" v-if="error.statusCode === 404"> خطای {{error.statusCode}}. <br>صفحه مورد نظر یافت نشد</h1>
            <h1 class="text-xl font-bold" v-else>Something Went Wrong.<br> Error: {{ error.statusCode }} </h1>
            <NuxtLink class="underline font-bold mt-5 text-cyan-400" to="/home">بازگشت به خانه</NuxtLink>
        </div>
    </div>
</template>

<script>
export default {
    props: ['error'],
    layout: 'homelayout'
  }
</script>