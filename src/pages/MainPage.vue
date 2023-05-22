<template>
  <div v-if="showPopup" class="popup-overlay" @click="closePopup">
    <div class="popup-content" @click.stop>
      <span class="close-icon" @click="closePopup">&times;</span>
      <div class="flex flex-col items-center">
        <h2 class="text-[45px] font-mono font-[600]">Специально для вас!!!</h2>
        <span class="text-[25px] font-mono font-[500] mb-2">
          ТОЛЬКО СЕГОДНЯ ДО КОНЦА ДНЯ</span
        >
        <img
          src="https://cdn3.mageplaza.com/media/general/MImGnKu.png"
          alt="akcija"
        />
        <button
          @click="closePopup"
          class="mt-4 text-[25px] font-[500] text-white bg-[#001d43] py-2.5 px-6 rounded-2xl"
        >
          Оставить Заявку!
        </button>
      </div>
      <!-- <form> -->
      <!-- Ваша форма здесь -->
      <!-- </form> -->
    </div>
  </div>
  <MainBlock @scrollToForm="scrollToForm" />
  <OfferBlock />
  <AboutUsBlock @scrollToForm="scrollToForm" />
  <ContactsBlock />
  <AchievementBlock />
  <FormBlock @addFormRef="addFormRef" />
  <Footer />
</template>

<script>
import MainTemplate from "@/components/layout/MainTemplate.vue";
import OfferBlock from "@/components/OfferBlock.vue";
import FormBlock from "@/components/FormBlock.vue";
import ContactsBlock from "@/components/ContactsBlock.vue";
import MainBlock from "@/components/MainBlock.vue";
import AchievementBlock from "@/components/AchievementBlock.vue";
import AboutUsBlock from "@/components/AboutUsBlock.vue";
import Header from "@/components/layout/Header.vue";
import Footer from "@/components/layout/Footer.vue";

export default {
  components: {
    Header,
    FormBlock,
    AchievementBlock,
    ContactsBlock,
    AboutUsBlock,
    OfferBlock,
    Footer,
    MainTemplate,
    MainBlock,
  },
  data() {
    return {
      formRef: null,
      showPopup: false,
    };
  },
  methods: {
    scrollToForm() {
      if (this.formRef) {
        const formElement = this.formRef;
        if (formElement) {
          formElement.scrollIntoView({ behavior: "smooth", block: "start" });
        }
      }
    },
    addFormRef(form) {
      this.formRef = form;
    },
    closePopup() {
      this.showPopup = false;
    },
  },
  mounted() {
    // setTimeout(() => {
    //   this.showPopup = true;
    // }, 1000);
  },

  watch: {
    showPopup(newValue, oldValue) {
      if (newValue) {
        document.querySelector("body").style.overflow = "hidden";
      } else {
        document.querySelector("body").style.overflow = "auto";
      }
    },
  },
};
</script>

<style>
.popup-overlay {
  z-index: 40 !important;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  align-items: center;
  justify-content: center;
}

.popup-content {
  z-index: 50 !important;
  background-color: white;
  padding: 20px;
  position: relative;
}

.close-icon {
  z-index: 100;
  position: absolute;
  top: 5px;
  right: 10px;
  cursor: pointer;
  font-size: 30px;
}
</style>
