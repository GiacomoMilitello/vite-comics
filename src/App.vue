<script>
import NavBar from "./components/NavBar.vue";
import ContentHere from "./components/ContentHere.vue";
import OurShop from "./components/OurShop.vue";

export default {
  components: {
    NavBar,
    ContentHere,
    OurShop
  },
};
</script>

<template>
  <NavBar />
  <ContentHere />
  <OurShop/>
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
