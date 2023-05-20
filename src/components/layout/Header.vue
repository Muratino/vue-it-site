<template>
  <header class="flex items-center justify-between mx-1">
    <div class="cursor-pointer">
      <img src="../../assets/img/Uslugi.svg" alt="logo" />
    </div>
    <nav class="max-[680px]:hidden">
      <ul class="flex items-center text-[20px] max-[1470px]:text-[16px]">
        <a class="cursor-pointer no-underline mr-[48px]">
          <li class="text-white  font-semibold">Услуги</li>
        </a>
        <a class="cursor-pointer no-underline mr-[48px]">
          <li class="text-white font-semibold">О нас</li>
        </a>
        <a class="cursor-pointer no-underline mr-[48px]">
          <li class="text-white font-semibold">
            Портфолио
          </li>
        </a>
        <a class="cursor-pointer no-underline mr-[48px]">
          <li class="text-white font-semibold">
            Решения
          </li>
        </a>
        <a class="cursor-pointer no-underline">
          <li class="text-white font-semibold">Контакты</li>
        </a>
      </ul>
    </nav>
    <div class="flex items-center text-white text-[18px] max-[1470px]:text-[15px] font-semibold max-[680px]:hidden">
      <span class="mr-1 cursor-pointer">EN</span>
      <span>/</span>
      <span class="ml-1 text-[#A7A7A7] cursor-pointer">UA</span>
    </div>
    <div class="hidden max-[680px]:block">
      <img class="w-[25px] h-[25px]" src="../../assets/img/menu-29.svg" alt="burger">
    </div>
  </header>
</template>


<!-- <script> -->
<!-- // export default {
//   data() {
//     return {
//       count: 0,
//     };
//   },
  // props: {
  //   posts: {
  //     type: Array,
  //     required: true
  //   },
// }; -->
<!-- </script> -->