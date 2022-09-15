<template>
    <div class="schedule-card text-xs w-full h-max rounded-xl bg-gray-100 p-3 py-4 flex gap-1 justify-between items-center">
        <div class="right flex flex-col justify-evenly gap-3">
            <div class="date flex gap-1">
                <p class="key">تاریخ شروع:</p>
                <p class="value">{{ schedule.date }}</p>
            </div>
            <div class="gym flex gap-1">
                <p class="key">باشگاه:</p>
                <p class="value">{{ schedule.gym }}</p>
            </div>
            <div class="coach flex gap-1">
                <p class="key">مربی:</p>
                <p class="value">{{ schedule.coach }}</p>
            </div>
        </div>
        <div class="left flex flex-col justify-between items-end gap-6 ">
            <div class="id flex gap-1">
                <p class="key">شماره برنامه:</p>
                <p class="value">{{ schedule.id }}</p>
            </div>
            <button class="p-1 px-3 border-[1px] border-black bg-transparent rounded-lg">
                مشاهده برنامه
            </button>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ScheduleCard',
    props: {
        schedule: Object
    }
}
</script>
<style scoped>
.key {
    color: black;
    font-weight: bold;
}
.value {
    color: rgb(113, 111, 111);
}
</style>