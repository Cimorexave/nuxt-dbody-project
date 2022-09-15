<template>
    <div dir="rtl" class="card absolute bottom-[10%]
    w-[80%] h-max shadow-md p-5 backdrop-blur-[15px] py-7
    text-sm flex flex-col gap-5">
        <header class="">
            <img src="~/assets/images/Group.png" alt="login card header logo">
        </header>
        <form class="input flex flex-col gap-5">
            <div class="text flex flex-col gap-1">
                <div class="input-label">
                    کد فعال سازی را وارد نمایید
                </div>
                <div class="help-number-text text-xs">
                    کد 6 رقمی ارسال شده به <span>09123456789</span> را وارد نمایید
                </div>
            </div>
            <input class=" p-1" placeholder="123456"
             type="number" minlength="6" maxlength="6" >
             <button @click.prevent type="submit" class="text-white bg-green-500 w-full p-2 rounded-full">
                ورود
             </button>
        </form>
        <nuxt-link to="/changephonenumber" class="change-phone-number underline">
            تغییر شماره موبایل
        </nuxt-link>
    </div>
</template>

<script>

    export default {
        name: 'LoginConfirmCard'
    }
</script>

<style scoped>
    .card {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    border-radius: 1rem;
    background: rgba( 255, 255, 255, 0.4 );
    box-shadow: 0 8px 32px 0 rgba(141, 141, 142, 0.37);
    border: 1px solid rgba( 255, 255, 255, 0.18 );
}
::placeholder {
    color: black;
}
    .card > * {
        opacity: 1;
        backdrop-filter: blur(0px) ;
        font-weight: lighter;
    }
    input {
        color: black;
        border: none;
        font-size: xx-large;
        letter-spacing: 1ch;
        background-color: transparent;
        border-bottom: 3px solid black;
    }
    input:focus {
        border: none;
    }
    input::placeholder {color: rgb(49, 49, 49);}
</style>