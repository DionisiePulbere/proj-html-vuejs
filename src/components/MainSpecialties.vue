<script> 
export default{
    name: "MainSpecialties",
    data(){
        return {

        }
    },

}
</script>

<template>
    <section>
        <div class="ms-container">
            <div class="container-page">
                <div class="text-center">
                    <h2>Our specialties<span class="brand-dot">.</span></h2>
                    <p class="gray-text">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    <div class="line"></div>
                </div>
                <div class="d-flex">
                    <div class="text-center">
                        <img src="../assets/img/svg/svg-0.svg" alt="">
                        <h3>Knowing</h3>
                        <p class="gray-text">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    </div>
                    <div class="text-center">
                        <img src="../assets/img/svg/svg-1.svg" alt="">
                        <h3>Selling</h3>
                        <p class="gray-text">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    </div>
                    <div class="text-center">
                        <img src="../assets/img/svg/svg-2.svg" alt="">
                        <h3>Learning</h3>
                        <p class="gray-text">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    </div>
                    <div class="text-center">
                        <img src="../assets/img/svg/svg-3.svg" alt="">
                        <h3>Contact</h3>
                        <p class="gray-text">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    </div>
                   
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
    position: relative;

    .ms-container{
        position: relative;
        top: -60px;
        background-color: white;
        width: 90%;
        margin: 0 auto;
        padding: 100px 0;
        .line{
            width: 70px;
            border-bottom: 2px solid $brand-primary;
            margin: 0 auto;
        }
        img{
            padding-top: 60px;
        }
        h3{
            padding: 16px 0;
        }
    }
    .btn-radious{
        bottom: 40px;
    }
}

</style>