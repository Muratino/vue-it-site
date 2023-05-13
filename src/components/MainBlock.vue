<template>
  <div class="w-full h-screen bg-[url('../assets/img/main-bg.svg')] bg-cover">
    <div class="max-w-[1050px] mr-auto ml-auto">
      <Header />
    </div>
    <div class="max-w-[1200px] mr-auto ml-auto">
      <div class="pt-[200px]">
        <h1 class="text-white font-semibold text-[48px] text-center p-0">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Ad, quia!
        </h1>
        <p class="text-[#ccced0] font-[300] text-[27px] text-center p-0">
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Consectetur
          aspernatur cum nisi reprehenderit pariatur quibusdam quis laudantium
          ea doloremque adipisci? Ipsa mollitia quas iusto quis, facilis sed
          veritatis possimus accusantium reiciendis doloribus officiis adipisci,
          voluptate suscipit nesciunt ullam blanditiis earum deserunt labore
          inventore aliquid iure.
        </p>
      </div>
      <div class="mt-36 flex items-center justify-center">
        <button
          class="transition-colors duration-200 ease-in-out text-white w-[351px] h-[72px] bg-[#536bb5] text-[24px] font-[500] text-center rounded-3xl cursor-pointer hover:bg-opacity-75"
        >
          Оставить заявку
        </button>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "./layout/Header.vue";

export default {
  components: {
    Header,
  },
};
</script>
