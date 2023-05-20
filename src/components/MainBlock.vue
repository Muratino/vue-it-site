<template>
  <div
    class="min-h-screen bg-[url('../assets/img/main-bg.svg')] bg-cover pt-10 pb-16 px-5 flex flex-col max-[1470px]:pt-7 max-[1470px]:pb-8 max-[1470px]:px-2 max-[1470px]:bg-auto max-[1470px]:bg-no-repeat"
  >
    <div class="max-w-[1050px] mx-auto w-full">
      <Header />
    </div>
    <div
      class="max-w-[1200px] mx-auto mt-4 text-center flex flex-auto flex-col justify-center items-center w-full max-[600px]:mt-10"
    >
      <h1
        class="text-white font-semibold text-[48px] p-0 max-[1470px]:text-[35px] max-[600px]:text-[25px]"
      >
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ad, quia!
      </h1>
      <p
        class="text-[#ccced0] font-[300] text-[27px] p-0 mt-2 max-[1470px]:text-[20px] max-[600px]:text-[15px]"
      >
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Consectetur
        aspernatur cum nisi reprehenderit pariatur quibusdam quis laudantium ea
        doloremque adipisci? Ipsa mollitia quas iusto quis, facilis sed
        veritatis possimus accusantium reiciendis doloribus officiis adipisci,
        voluptate suscipit nesciunt ullam blanditiis earum deserunt labore
        inventore aliquid iure.
      </p>
      <button
        class="transition-colors duration-200 ease-in-out text-white w-full max-w-[350px] py-3.5 mt-16 bg-[#536bb5] text-[24px] font-[500] text-center rounded-3xl cursor-pointer hover:bg-opacity-75 max-[1470px]:text-[20px] max-[1470px]:py-2.5 max-[1470px]:max-w-[250px] max-[400px]:text-[16px] max-[400px]:max-w-[200px]"
      >
        Оставить заявку
      </button>
    </div>
  </div>
</template>

<script>
import Header from "./layout/Header.vue";

export default {
  components: {
    Header,
  },
  // data() {
  //   return {
  //     count: 0,
  //   };
  // },
  // props: {
  //   posts: {
  //     type: Array,
  //     required: true
  //   },
};
</script>
