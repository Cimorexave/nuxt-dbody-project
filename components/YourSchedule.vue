<template>
  <div class="your-schedule w-full flex flex-col gap-3 pb-16">
    <div v-for="schedule in schedules" :key="schedule.id">
      <ScheduleCard :schedule="schedule" />
    </div>
  </div>
</template>
<script>
import ScheduleCard from "~/components/ScheduleCard.vue";

export default {
  name: "YourSchedule",
  components: {
    ScheduleCard,
  },
  data() {
    return {
      schedules: [
        {
          id: 1,
          gym: "اکسیژن",
          date: "15 اردیبهشت 1401",
          coach: "هادی چوپان",
        },
        {
          id: 2,
          gym: "اکسیژن",
          date: "4 فروردین 1401",
          coach: "هادی چوپان",
        },
        {
          id: 3,
          gym: "اکسیژن",
          date: "3 مهر 1401",
          coach: "هادی چوپان",
        },
        {
          id: 4,
          gym: "اکسیژن",
          date: "25 خرداد 1401",
          coach: "هادی چوپان",
        },
      ],
    };
  },
};
</script>
