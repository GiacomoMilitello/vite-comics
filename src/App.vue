<script>
import NavBar from "./components/NavBar.vue";
import JumboTitles from "./components/JumboTitles.vue";
import OurShop from "./components/OurShop.vue";
import FooterLinks from "./components/FooterLinks.vue";
import SignUp from "./components/SignUp.vue";

export default {
  components: {
    NavBar,
    JumboTitles,
    OurShop,
    FooterLinks,
    SignUp
  },
};
</script>

<template>
  <NavBar />
  <JumboTitles/>
  <OurShop/>
  <FooterLinks/>
  <SignUp/>
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
