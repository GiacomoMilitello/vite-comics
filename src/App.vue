<script>
import NavBar from "./components/NavBar.vue";
import ContentHere from "./components/ContentHere.vue";

export default {
  components: {
    NavBar,
    ContentHere,
  },
};
</script>

<template>
  <NavBar />
  <ContentHere />
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
