<script>
    export default{
    name: "MainGallery",

    }

</script>

<template>
    <section class="gallery">
        <div class="buttons">
            <div class="logo mb-2">
                <img class="p-2" src="../assets/img/svg/svg-5.svg" alt="">
            </div>
            <div class="cart">
                <img class="p-2" src="../assets/img/svg/svg-7.svg" alt="">
            </div>
        </div>
        <div class="btn-radious">
                <i class="fa-solid fa-arrow-up-long"></i>
            </div>
        <div class="container-fluid">
            <i class="fa-solid fa-play"></i>
            <img src="../assets/img/h1-img-04.jpg" alt="">
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

img{
    width: 100%;
}
.container-fluid{

    i{
        font-size: 50px;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50% , -50%);
        color: white;       
    }
}
section{
    position: relative;
}

.btn-radious{
    top: 20%;
}
.buttons{
    position: absolute;
    top: -20px;
    right: 0;
    background-color: transparent;
    img{
        width: 40px;
    }
}

.cart{
    background-color: white;
}

.logo{
    background-color: $brand-primary;
}
</style>