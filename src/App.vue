<script>
import NavBar from "./components/NavBar.vue";
import ContentHere from "./components/ContentHere.vue";
import OurShop from "./components/OurShop.vue";
import FooterLinks from "./components/FooterLinks.vue";
import SignUp from "./components/SignUp.vue";

export default {
  components: {
    NavBar,
    ContentHere,
    OurShop,
    FooterLinks,
    SignUp
  },
};
</script>

<template>
  <NavBar />
  <ContentHere />
  <OurShop/>
  <FooterLinks/>
  <SignUp/>
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
