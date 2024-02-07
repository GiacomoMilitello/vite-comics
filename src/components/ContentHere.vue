<script>
export default {
  name: "ContentHere",
  
};
</script>

<template>
  <div id="content-here" class="d-flex align-items-center ">
    <h2 class="text-white w-75 mx-auto">
        --> Content goes here <--
    </h2>
  </div>

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;
    #content-here{
        height: 74px;
        background-color: black;
    }

</style>
