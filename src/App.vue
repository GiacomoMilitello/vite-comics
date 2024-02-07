<script>
import NavBar from "./components/NavBar.vue";
import ContentHere from "./components/ContentHere.vue";
import OurShop from "./components/OurShop.vue";
import FooterLinks from "./components/FooterLinks.vue";

export default {
  components: {
    NavBar,
    ContentHere,
    OurShop,
    FooterLinks
  },
};
</script>

<template>
  <NavBar />
  <ContentHere />
  <OurShop/>
  <FooterLinks/>
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
