<template>
  <section dir="rtl" class="home-content flex flex-col items-center p-5 gap-5">
    <div class="input relative w-full">
      <input
        type="text"
        placeholder="جست و جو..."
        class="rounded-full bg-gray-200 p-3 py-2 text-sm w-full border-0"
      />
      <i class="el-icon-search absolute left-5 top-[30%] font-bold text-lg"></i>
    </div>
    <img src="~/assets/images/ad banner.png" alt="ad picture" class="ad" />
    <div class="inline-nav flex flex-row gap-2 justify-evenly h-max w-full">
      <div
        @click="tabSwitcher(item.id)"
        class="el"
        v-for="item of navbarTabs"
        :key="item.id + '_navbarTabs_'"
      >
        <div
          class="inline-nav-el inline-nav-el-1"
          :class="item.id === tabNavNumber && 'is-active'"
        ></div>
        <div class="el-label">{{ item.title }}</div>
      </div>
    </div>
    <div class="tabs w-full">
      <YourSchedule v-if="tabNavNumber === 0" />
      <Instructions v-if="tabNavNumber === 1" />
      <OrderPlan v-if="tabNavNumber === 2" />
      <Shop v-if="tabNavNumber === 3" />
    </div>
  </section>
</template>
<script>
export default {
  name: "HomeContentComponent",
  data() {
    return {
      tabNavNumber: 0,
      navbarTabs: [
        {
          title: "برنامه‌های شما",
          img: "/images/1.png",
          id: 0,
        },
        {
          title: "آموزش",
          img: "/images/1.png",
          id: 1,
        },
        {
          title: "سفارش برنامه",
          img: "/images/1.png",
          id: 2,
        },
        {
          title: "فروشگاه",
          img: "/images/1.png",
          id: 3,
        },
      ],
    };
  },
  methods: {
    tabSwitcher(tabId) {
      this.tabNavNumber = tabId;
    },
  },
};
</script>
<style scoped>
.el {
  width: 25%;
  display: flex;
  flex-direction: column;
  flex-basis: 25%;
  gap: 0.5em;
}
input:focus { border: none }
.inline-nav-el {
  background-color: rgb(222, 222, 222);
  opacity: 0.8;
  border-radius: 0.5rem;
  width: 100%;
  display: grid;
  aspect-ratio: 1;
}
.el-label {
  text-align: center;
  font-size: 0.5rem;
}
.is-active {
  background-color: black;
}
</style>
