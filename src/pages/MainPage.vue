<template>
  <MainBlock />
  <OfferBlock />
  <AboutUsBlock />
  <ContactsBlock />
  <AchievementBlock />
  <FormBlock />
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
};
</script>

<style></style>
