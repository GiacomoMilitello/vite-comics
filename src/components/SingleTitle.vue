<script>
export default {
  name: "SingleTitle",
  props: {
    propsThumb: String,
    propsSeries: String
  }
};
</script>

<template>
  
  <div class="col-2">
        <figure v-bind:style="{ backgroundImage: 'url(' + propsThumb + ')' }">
        </figure>
        <h4 class="text-uppercase text-white pt-3 pb-5">{{ propsSeries }}</h4>
    </div>

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

    figure{
        aspect-ratio: 1;
        background-position: top;
        background-repeat: no-repeat;
        background-size: cover;
    }
    h4{
        font-size: 90%;
    }
</style>