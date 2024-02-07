<script>
export default {
  name: "FooterLinks",
    data() {
        return {
            comics: [
                { name: 'Characters' },
                { name: 'Comics' },
                { name: 'Movies' },
                { name: 'TV' },
                { name: 'Games' },
                { name: 'Videos' },
                { name: 'News' }
            ],
            shops: [
                { name: 'Shop DC' },
                { name: 'Shop DC Collectibles' }
            ],
            dc: [
                { name: 'Terms Of Use' },
                { name: 'Privacy policy (New)' },
                { name: 'Ad Choices' },
                { name: 'Advertising' },
                { name: 'Jobs' },
                { name: 'Subscriptions' },
                { name: 'Talent Workshops' },
                { name: 'CPSC Certificates' },
                { name: 'Ratings' },
                { name: 'Shop Help' },
                { name: 'Contact Us' }
            ],
            sites: [
                { name: 'DC' },
                { name: 'MAD Magazine' },
                { name: 'DC Kids' },
                { name: 'DC Universe' },
                { name: 'DC Power Visa' }
            ]            
        }
    }
  
};
</script>

<template>
    <div id=footer-links>
        <div class="w-75 mx-auto row">
            <div class="col-6 py-5 d-flex gap-5">
                <div class="d-flex flex-column gap-4">
<!-- DC COMICS -->
                    <ul class="list-unstyled">
                        <li class="text-white fw-bold">DC COMICS</li>
                        <li v-for="element in comics" :key="element.name" class="">
                            <a class="text-decoration-none d-flex align-items-center text-white opacity-50 fw-light" aria-current="page" href="#">{{element.name}}</a>
                        </li>
                    </ul>
<!-- SHOP -->
                    <ul class="list-unstyled">
                        <li class="text-white fw-bold">SHOP</li>
                        <li v-for="shop in shops" :key="shop.name" class="">
                            <a class="text-decoration-none d-flex align-items-center text-white opacity-50 fw-light" aria-current="page" href="#">{{shop.name}}</a>
                        </li>
                    </ul>
                </div>
<!-- SHOP -->
                <ul class="list-unstyled">
                    <li class="text-white fw-bold">DC</li>
                    <li v-for="contact in dc" :key="contact.name" class="">
                        <a class="text-decoration-none d-flex align-items-center text-white opacity-50 fw-light" aria-current="page" href="#">{{contact.name}}</a>
                    </li>
                </ul>
<!-- SITES -->
                <ul class="list-unstyled">
                    <li class="text-white fw-bold">SITES</li>
                    <li v-for="site in sites" :key="site.name" class="">
                        <a class="text-decoration-none d-flex align-items-center text-white opacity-50 fw-light" aria-current="page" href="#">{{site.name}}</a>
                    </li>
                </ul>
            </div>
            <div id="dc-logo" class="col-6"></div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

    #footer-links{
        background-image: url(../img/footer-bg.jpg);
    }
    #dc-logo{
            background-image: url(../img/dc-logo-bg.png);
            background-position: center;
            background-repeat: no-repeat;
            background-size: cover;
            }
    a{
        border-bottom: 1px solid transparent;
                    &:hover {
                        color: $dc-color;
                        border-bottom: 1px solid white;
                    }
    }

</style>