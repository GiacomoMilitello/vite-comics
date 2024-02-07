<script>
export default {
    name: "SignUp",
    data() {
        return {
            socials: [
                {image: 'src/img/footer-facebook.png' 
                },
                {image: 'src/img/footer-twitter.png' 
                },
                {image: 'src/img/footer-youtube.png' 
                },
                {image: 'src/img/footer-pinterest.png' 
                },
                {image: 'src/img/footer-periscope.png' 
                }
            ]
        }
    }
};
</script>

<template>
  <div id="sign-up" class="">
    <div class="w-75 mx-auto py-4 d-flex justify-content-between align-items-center ">
        <button type="button" class="py-2 px-3">SIGN-UP-NOW!</button>
        <ul class="d-flex list-unstyled gap-3">
            <li class="fw-bold d-flex align-items-center ">FOLLOW US</li>
            <li v-for="social in socials" :key="social.image" class="py-4">
            <a class="text-decoration-none text-uppercase d-flex align-items-center text-white gap-3 " aria-current="page" href="#">
                <figure>
                    <img class="img-fluid" :src="social.image" alt="Social image">
                </figure>
            </a>
        </li>
        </ul>
    </div>
  </div>

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

    #sign-up{
        background-color: #333333;
        button{
            border: 1px solid $dc-color;
            background-color: transparent;
            color: white;
            &:hover {
            color: $dc-color;
            border: 1px solid white;
            }
        }
        li{
            color: $dc-color;
            figure{
                width: 25px;
            }
        }
    }

</style>