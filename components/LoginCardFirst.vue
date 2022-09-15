<!-- login card  -->
<template>
    <div dir="rtl" class="card absolute bottom-[10%]
    w-[80%] h-max py-7 shadow-md p-5 backdrop-blur-[15px]
    text-sm flex flex-col gap-5">
        <header class="">
            <img src="~/assets/images/Group.png" alt="login card header logo">
        </header>
        <form class="input flex flex-col gap-5">
            <div class="input-label">
                شماره موبایل خود را وارد نمایید
            </div>
            <input class="bg-transparent p-4 border-b-2 text-black  border-black "
             type="text" placeholder="مثلا 09123456789">
             <button @click.prevent type="submit" class="text-white bg-green-500 w-full p-2 rounded-full">
                ورود
             </button>
        </form>
        <div class="warning text-[0.6rem]">
            عضویت به معنای پذیرش <nuxt-link to="/policies" class="text-green-500 underline">قوانین و مقررات </nuxt-link> می‌باشد
        </div>
    </div>
</template>

<script>


    export default {
        name: "LoginCardFirst"
    }
</script>

<style scoped>
.card {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    border-radius: 1rem;
    background: rgba( 255, 255, 255, 0.4);
    box-shadow: 0 8px 32px 0 rgba(141, 141, 142, 0.37);
    border: 1px solid rgba( 255, 255, 255, 0.18 );
}
::placeholder {
    color: black;
}
</style>