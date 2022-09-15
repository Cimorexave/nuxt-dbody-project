<template>
    <div dir="rtl" class="signup flex flex-col bg-white text-black w-full h-full
    p-5 py-7 items-center gap-8">
        <img src="~/assets/images/Group.png" alt="logo">
        <div class="description text-lg">
            لطفا اطلاعات خواسته شده را تکمیل نمایید:
        </div>
        <form @click.prevent="submitForm"
         class="signup-form flex flex-col gap-5 w-[90%]">
            <input class="first-name"  placeholder="نام" />

            <input class="last-name"  placeholder="نام خانوادگی" />
            
            <input class="code-melli"  placeholder="کد ملی" />
            
            <input class="career"  placeholder="شغل" />
            
            <div class="gender">
                <label for="gender">جنسیت : </label>
                <select name="gender" id="gender">
                    <option value="male">مرد</option>
                    <option value="female">زن</option>
                </select>
            </div>
            
            <input type="date" class="birthday"  placeholder="تاریخ تولد" />
        </form>
        <button type="submit" @click.prevent="open2"
        class="singup-btn rounded-full text-white bg-green-500 p-3 w-[80%]">
            ثبت اطلاعات
        </button>
    </div>
</template>
<script>

    export default {
        name: 'SignupComponent',
        data() {
            user: {
                firstName: "";
                lastName: "";
                codeMelli: 0;
                carrer: "";
                gender: "";
                birthday: "";
            }
        },
        methods: {
            open2() {
                this.$message({
                    message: 'اطلاعات شما با موفقیت ثبت شد',
                    type: 'success'
                });
            },
            submitForm() {
            }
        }
    }
</script>
<style>
    input {
        border-bottom: 2px solid black;
        width: 100%;
        padding: 0.5rem;
    }
</style>