<template>
  <div
    ref="offers"
    class="min-h-screen bg-[url('../assets/img/bg-offer.svg')] bg-auto bg-right bg-no-repeat pt-5 pb-10 px-5 flex flex-col max-[1470px]:pt-7 max-[1470px]:pb-8 max-[1470px]:px-2 max-[1470px]:bg-auto max-[1470px]:bg-no-repeat"
  >
    <div class="max-w-[1200px] mx-auto w-full">
      <div class="flex items-start justify-center relative">
        <h2
          class="p-0 text-[120px] text-[#C3C3C3] font-[800] text-opacity-50 max-[1000px]:text-[90px] max-[600px]:text-[65px]"
        >
          УСЛУГИ
        </h2>
        <span
          class="text-black text-[32px] font-[700] absolute top-16 max-[1000px]:text-[27px] max-[600px]:text-[20px] max-[600px]:top-10"
          >Высокое качество услуг</span
        >
      </div>
      <div
        class="grid gap-y-8 gap-x-6 grid-cols-8 grid-rows-4 mt-10 mx-2 max-[1020px]:gap-6 max-[1020px]:grid-cols-6 max-[675px]:grid-cols-2 max-[675px]:grid-rows-none max-[675px]:gap-2"
      >
        <div
          class="col-start-1 col-end-3 flex flex-col items-center mr-10 text-[24px] max-[820px]:text-[20px] max-[520px]:text-[17px] max-[350px]:text-[14px] max-[675px]:col-start-auto max-[675px]:col-end-auto"
        >
          <img
            class="max-[520px]:w-[65px] max-[360px]:w-[55px]"
            src="../assets/img/1.svg"
            alt="img"
          />
          <span class="text-[#4d5165] font-[600] max-[820px]:text-[#26272b]"
            >IT Консультирование</span
          >
        </div>
        <div
          class="col-start-3 col-end-6 text-[24px] max-[675px]:col-end-auto max-[675px]:col-start-auto flex flex-col items-center max-[820px]:text-[20px] max-[520px]:text-[17px] max-[350px]:text-[14px] max-[800px]:text-[#8489a1]"
        >
          <img
            class="max-[520px]:w-[65px] max-[360px]:w-[55px]"
            src="../assets/img/2.svg"
            alt="img"
          />
          <span class="text-[#4d5165] font-[600] max-[820px]:text-[#26272b]"
            >Разработка ПО под заказ</span
          >
        </div>
        <div
          class="col-start-6 col-end-8 text-[24px] max-[675px]:col-end-auto max-[675px]:col-start-auto flex flex-col items-center max-[820px]:text-[20px] max-[520px]:text-[17px] max-[350px]:text-[14px] max-[800px]:text-[#8489a1] mt-2"
        >
          <img
            class="max-[520px]:w-[65px] max-[360px]:w-[55px]"
            src="../assets/img/3.svg"
            alt="img"
          />
          <span class="text-[#4d5165] font-[600] max-[820px]:text-[#26272b]"
            >Оффшор разработка</span
          >
        </div>
        <div
          class="col-start-2 col-end-4 text-[24px] max-[675px]:col-end-auto max-[675px]:col-start-auto flex flex-col items-center max-[820px]:text-[20px] max-[520px]:text-[17px] max-[350px]:text-[14px] max-[800px]:text-[#8489a1] mt-2"
        >
          <img
            class="max-[520px]:w-[65px] max-[360px]:w-[55px]"
            src="../assets/img/4.svg"
            alt="img"
          />
          <span class="text-[#4d5165] font-[600] max-[820px]:text-[#26272b]"
            >Поддержка ПО</span
          >
        </div>
        <div
          class="col-start-4 col-end-8 text-[24px] max-[675px]:col-end-auto max-[675px]:col-start-auto flex flex-col items-center max-[820px]:text-[20px] max-[520px]:text-[17px] max-[350px]:text-[14px] max-[800px]:text-[#8489a1] mt-2"
        >
          <img
            class="max-[520px]:w-[65px] max-[360px]:w-[55px]"
            src="../assets/img/5.svg"
            alt="img"
          />
          <span class="text-[#4d5165] font-[600] max-[820px]:text-[#26272b]"
            >Услуги R&D</span
          >
        </div>
        <div
          class="col-start-1 col-end-3 text-[24px] max-[675px]:col-end-auto max-[675px]:col-start-auto flex flex-col items-center max-[820px]:text-[20px] max-[520px]:text-[17px] max-[350px]:text-[14px] max-[800px]:text-[#8489a1] mt-2"
        >
          <img
            class="max-[520px]:w-[65px] max-[360px]:w-[55px]"
            src="../assets/img/6.svg"
            alt="img"
          />
          <span class="text-[#4d5165] font-[600] max-[820px]:text-[#26272b]"
            >QA и тестирование</span
          >
        </div>
        <div
          class="col-start-3 col-end-6 text-[24px] max-[675px]:col-end-auto max-[675px]:col-start-auto flex flex-col items-center max-[820px]:text-[20px] max-[520px]:text-[17px] max-[350px]:text-[14px] max-[800px]:text-[#8489a1] mt-2"
        >
          <img
            class="max-[520px]:w-[65px] max-[360px]:w-[55px]"
            src="../assets/img/7.svg"
            alt="img"
          />
          <span class="text-[#4d5165] font-[600] max-[820px]:text-[#26272b]"
            >DevOps услуги</span
          >
        </div>
        <div
          class="col-start-1 col-span-4 text-[24px] max-[675px]:col-end-auto max-[675px]:col-start-auto flex flex-col items-center max-[820px]:text-[20px] max-[520px]:text-[17px] max-[350px]:text-[14px] max-[800px]:text-[#8489a1] mt-2"
        >
          <img
            class="max-[520px]:w-[65px] max-[360px]:w-[55px]"
            src="../assets/img/8.svg"
            alt="img"
          />
          <span class="text-[#4d5165] font-[600] max-[820px]:text-[#26272b]"
            >Разработка UI/UX дизайна</span
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { objOfName } from "../pages/MainPage.vue";
export default {
  mounted() {
    this.$emit("addSomeRef", {
      ref: this.$refs.offers,
      name: objOfName.offers,
    });
  },
};
</script>
