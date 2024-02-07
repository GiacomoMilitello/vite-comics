<script>
export default {
  name: "NavBar",
  data(){
    return {
      links: [
        { name: 'characters' },
        { name: 'comics' },
        { name: 'movies' },
        { name: 'tv' },
        { name: 'games' },
        { name: 'collectibles' },
        { name: 'videos' },
        { name: 'fans' },
        { name: 'news' },
        { name: 'shop' }
      ]
    }
  }
};
</script>

<template>
  <nav class="w-75 mx-auto d-flex align-items-center justify-content-between">
    <figure class="">
      <img class="img-fluid" src="../img/dc-logo.png" alt="">
    </figure>
    <ul class="d-flex list-unstyled gap-4">
        <li v-for="link in links" :key="link.name" class="fw-bold">
          <a class="text-decoration-none text-uppercase d-flex align-items-center" aria-current="page" href="#">{{link.name}}</a>
        </li>
      </ul>
  </nav>

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

nav{
  figure{
      width: 60px;
      height: 60px;
  }
  ul{
    height: 90px;
    li{
      height: 90px;
      a{
        height: 90px;
        color: black;
        border-bottom: 5px solid transparent;
        &:hover {
          color: $dc-color;
          border-bottom: 5px solid $dc-color;
        }
      }
    }
  }
}

</style>
