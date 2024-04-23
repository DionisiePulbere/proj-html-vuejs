<script>
    export default{
    name: "MainFounder",

    }

</script>

<template>
<section class="founder">
    <div class="container-page d-flex">
        <div class="col-7 left">
            <img src="../assets/img/h1-img-01.jpg" alt="">
            <div class="arrows d-flex">
                <i class="fa-solid fa-arrow-left-long"></i>
                <i class="fa-solid fa-arrow-right-long"></i>
            </div>
        </div>
        <div class="col-7 right">
            <h2>Jason Bickford</h2>
            <p class="gray-text">Founder and Execution Director</p>
            <div class="line-70"></div>
            <p class="gray-text pt-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            <div class="d-flex social">
                <i class="fa-brands fa-linkedin-in"></i>
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-twitter"></i>
            </div>
        </div>
    </div>
    <div class="btn-radious">
        <i class="fa-solid fa-arrow-up-long"></i>
    </div>
</section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;
section{
    padding-bottom: 100px;
    position: relative;
    .arrows {
        position: absolute;
        bottom: 0;
        left: 0;

        i{
            background-color: $brand-primary;
            color: white;
            padding: 20px;
        }
    }
}

img{
    width: 100%;
}

.left{
    position: relative;

}

.right{
    position: relative;
    top: 40px;
    left: -100px;
    padding: 70px 50px;
    background-color: white;
    height: 80%;
}

</style>
