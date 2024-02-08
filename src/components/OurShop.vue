<script>
export default {
  name: "OurShop",
    data() {
        return {
            shops: [
                { name: 'digital comics',
                image: 'src/img/buy-comics-digital-comics.png' 
                },
                { name: 'dc merchandise',
                image: 'src/img/buy-comics-merchandise.png' 
                },
                { name: 'subscription',
                image: 'src/img/buy-comics-subscriptions.png' 
                },
                { name: 'comic shop locator',
                image: 'src/img/buy-comics-shop-locator.png' 
                },
                { name: 'dc power visa',
                image: 'src/img/buy-dc-power-visa.svg' 
                }
            ]
        }
    }
};
</script>

<template>
  <div id="our-shop" class="">
    <ul class="d-flex justify-content-between  list-unstyled gap-4 w-75 mx-auto">
        <li v-for="shop in shops" :key="shop.name" class="">
            <a class="text-decoration-none text-uppercase d-flex align-items-center text-white gap-3 py-4" aria-current="page" href="#">
                <figure :style="{ backgroundImage: 'url(' + shop.image + ')' }"></figure>
                {{shop.name}}
            </a>
        </li>
      </ul>
  </div>
  

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;
    
    #our-shop{
        background-color: $dc-color;
        ul{
            li{
                a{
                    font-size: 85%;
                    border-bottom: 3.5px solid transparent;
                    &:hover {
                        color: $dc-color;
                        border-bottom: 3.5px solid white;
                    }
                    figure{
                        width: 40px;
                        height: 40px;
                        @include background-contain;
                    }
                }
            }
        }
    }

</style>