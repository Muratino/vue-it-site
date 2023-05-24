<template>
  <div
    ref="contacts"
    class="h-full max-h-[1000px] bg-[url('../assets/img/contacts-bg.png')] bg-cover px-2 py-10 mt-[100px] mb-[50px]"
  >
    <div class="max-w-[1200px] mx-auto">
      <div
        class="flex items-center justify-between max-[770px]:flex-col max-[770px]:justify-center"
      >
        <div class="relative w-full max-[770px]:mb-10">
          <div class="absolute top-[-300px] max-[770px]:static">
            <div
              class="bg-[#132641] w-full flex flex-col items-center py-[20px] px-[25px] h-[600px] max-[770px]:h-auto max-[770px]:flex-row max-[430px]:flex-col"
            >
              <div>
                <h2
                  class="p-0 text-[50px] text-[#224880] font-[800] text-center max-[1000px]:text-[38px] max-[850px]:text-[30px] max-[590px]:text-[24px]"
                >
                  КАК СВЯЗАТСЯ С НАМИ?
                </h2>
                <p
                  class="p-0 text-[30px] text-white font-[500] text-center mt-4 max-[1000px]:text-[26px] max-[1000px]:mt-1 max-[850px]:text-[24px] max-[590px]:text-[18px]"
                >
                  PNN SOFT, UKRAINE
                </p>
                <div class="flex items-start mt-6 max-[1000px]:mt-3">
                  <img
                    class="mr-2 max-[770px]:mr-1 max-[590px]:w-[20px]"
                    src="../assets/img/Mask group.svg"
                    alt="icon"
                  />
                  <span
                    class="p-0 text-[22px] text-[#A9A9A9] font-[400] text-center max-[1000px]:text-[18px] max-[590px]:text-[14px]"
                    >Украина, Киев, 03062 просп. Победы, 67 Корпус Е</span
                  >
                </div>
              </div>

              <div class="mt-6 max-[770px]:mt-2">
                <img src="../assets/img/dddd.png" alt="map" />
              </div>
            </div>
          </div>
        </div>

        <div
          class="p-2 max-[770px]:grid max-[770px]:grid-cols-3 gap-3 max-[695px]:grid-cols-2 max-[695px]:gap-5 max-[390px]:grid-cols-1"
        >
          <div class="flex items-center justify-between mb-10 max-[770px]:mb-1">
            <div
              class="w-[50px] h-[50px] max-[770px]:w-[30px] max-[770px]:h-[30px] rounded-full bg-[#122D55] flex items-center justify-center"
            >
              <img
                class="max-[770px]:w-[20px]"
                src="../assets/img/phone.svg"
                alt="icon"
              />
            </div>
            <span
              class="text-[20px] font-[500] text-white max-[850px]:text-[17px] max-[470px]:text-[13px]"
              >+ 48 534 565 194 <br />
              +48 465 221 890</span
            >
          </div>
          <div class="flex items-center justify-between mb-10 max-[770px]:mb-1">
            <div
              class="w-[50px] h-[50px] max-[770px]:w-[30px] max-[770px]:h-[30px] rounded-full bg-[#122D55] flex items-center justify-center"
            >
              <img
                class="max-[770px]:w-[20px]"
                src="../assets/img/email.svg"
                alt="icon"
              />
            </div>
            <span
              class="text-[20px] font-[500] text-white max-[850px]:text-[17px] max-[470px]:text-[13px]"
              >info@gmail.com</span
            >
          </div>
          <div class="flex items-center justify-between mb-10 max-[770px]:mb-1">
            <div
              class="w-[50px] h-[50px] max-[770px]:w-[30px] max-[770px]:h-[30px] rounded-full bg-[#122D55] flex items-center justify-center"
            >
              <img
                class="max-[770px]:w-[20px]"
                src="../assets/img/twitter.svg"
                alt="icon"
              />
            </div>
            <span
              class="text-[20px] font-[500] text-white max-[850px]:text-[17px] max-[470px]:text-[13px]"
              >twitterground.com</span
            >
          </div>
          <div class="flex items-center justify-between mb-10 max-[770px]:mb-1">
            <div
              class="w-[50px] h-[50px] max-[770px]:w-[30px] max-[770px]:h-[30px] rounded-full bg-[#122D55] flex items-center justify-center mr-2"
            >
              <img
                class="max-[770px]:w-[20px]"
                src="../assets/img/insta.svg"
                alt="icon"
              />
            </div>
            <span
              class="text-[20px] font-[500] text-white max-[850px]:text-[17px] max-[470px]:text-[13px]"
              >instagram.infolink.com</span
            >
          </div>
          <div class="flex items-center justify-between">
            <div
              class="w-[50px] h-[50px] max-[770px]:w-[30px] max-[770px]:h-[30px] rounded-full bg-[#122D55] flex items-center justify-center"
            >
              <img
                class="max-[770px]:w-[20px]"
                src="../assets/img/messanger.svg"
                alt="icon"
              />
            </div>
            <span
              class="text-[20px] font-[500] text-white max-[850px]:text-[17px] max-[470px]:text-[13px]"
              >info.watsapp.com</span
            >
          </div>
          <div class=""></div>
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
      ref: this.$refs.contacts,
      name: objOfName.contacts,
    });
  },
};
</script>
