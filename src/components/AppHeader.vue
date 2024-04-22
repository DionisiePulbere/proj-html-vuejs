<script>
import AppHero from "./AppHero.vue"

   export default{
        name: 'AppHeader',
        components: {
        AppHero,

    },
        data() {
            return {
                navLinks: ["homes", "pages", "blog", "shop", "events", "elements"],
                isActive: 0, 
            }
        },
        methods: {
            thisIsActive(index) {
                this.isActive= index;            }
        }
    }
</script>

<template>
    <header>
        <div class="ms-container">
            <div class="logo">
                <a href="#">
                    <img src="../assets/img/logo-img-01.png" alt="">
                </a>
            </div>
            <nav>
                <ul class="d-flex ">
                    <li v-for="link, index in navLinks"><a href="#" class="mx-3"  :class="{ 'active': isActive === index }" @click="thisIsActive(index)" ><i class="fa-solid fa-arrow-right-long mx-2"></i>{{ link }}</a></li>
                    <li><a href="#"><i class="mx-3 fa-solid fa-magnifying-glass"></i></a></li>
                    <li><a href="#"><i class="mx-3 fa-solid fa-list-ul"></i></a></li>
                </ul>
            </nav>
        </div>
    </header>
    <AppHero></AppHero>
</template>

<style scoped lang="scss">
@use '../style/generic' as *;
@use '../style/partials/variables' as *;
header{
    background-color: transparent;
    position: relative;
    z-index: 10;
}

.ms-container{
    display: flex;
    justify-content: space-between;
    margin: 30px 60px;
    text-transform: uppercase;
    .logo a img{
        width: 150px;
    }
}

i.fa-magnifying-glass{
    transform: scaleX(-1);
}
i.fa-arrow-right-long{
    display: none;
}

.active{
    color: $brand-primary;
    display: flex;
    align-items: center;
    .fa-arrow-right-long{
        display: block;
    }
}  
</style>