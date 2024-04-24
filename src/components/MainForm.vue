<script>
    export default{
    name: "MainForm",

    }

</script>

<template>
    <section class="contact py-5">
        <div class="container-page d-flex">
            <div class="map col-6 py-5 me-5">
                <div class="post-it">
                    <h5>New York Coaching</h5>
                    <div class="more">read more</div>
                </div>
                <div class="dot-1">
                    <img src="../assets/img/h1-contact-rev-02.png" alt="">
                </div>
                <div class="dot-2">
                    <img src="../assets/img/h1-contact-rev-02.png" alt="">
                </div>
                <div class="dot-3">
                    <img src="../assets/img/h1-contact-rev-02.png" alt="">
                </div>
                <img src="../assets/img/h1-contact-rev-01.png" alt="">
            </div>
            <div class="col-6">
                <h2>Contact us<span class="brand-dot">.</span></h2>
                <p class="gray-text">Lorem ipsum dolor sit amet consectetur, adipisicing elit. </p>
                <div class="line-70"></div>
                <div class="d-flex my-3">
                    <div class="col-6 my-3 pe-3">
                        <input type="text"  placeholder="Your Name">
                    </div>
                    <div class="col-6 my-3">
                        <input type="text"  placeholder="Your Name">
                    </div>
                </div>
                 <div class="col-12 mb-3">
                    <textarea placeholder="Write a message..." rows="3"></textarea>
                </div>
                <button class="ms-btn ms-btn-secondary mt-4">send<span class="line">|</span><i class="ps-3 fa-solid fa-arrow-right-long"></i></button>
            </div>
            <div class="logos d-flex">
                <div class="col-20">
                    <img src="../assets/img/h4-clients-img-03.png" alt="">
                </div>
            </div>
        </div>
        <div class="container-page d-flex">
            <div class="col-20">
                <img class="dis" src="../assets/img/h4-clients-img-03.png" alt="">
                <img class="hover" src="../assets/img/h4-clients-img-04-1.png" alt="">
            </div>
            <div class="col-20">
                <img class="dis" src="../assets/img/h4-clients-img-05.png" alt="">
                <img class="hover" src="../assets/img/h4-clients-img-06-1.png" alt="">
            </div>
            <div class="col-20">
                <img class="dis" src="../assets/img/h4-clients-img-07.png" alt="">
                <img class="hover" src="../assets/img/h4-clients-img-08-1.png" alt="">
            </div>
            <div class="col-20">
                <img class="dis" src="../assets/img/h4-clients-img-09.png" alt="">
                <img class="hover" src="../assets/img/h4-clients-img-10-1.png" alt="">
            </div>
            <div class="col-20">
                <img class="dis" src="../assets/img/h4-clients-img-01.png" alt="">
                <img class="hover" src="../assets/img/h4-clients-img-02.png" alt="">
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;
img{
    width: 100%;
}

.col-20{
width: 20%;
padding: 40px;
    .hover{
    display: none;
    }
    img{
        color: black;
        width: 100%;
    }
    &:hover .hover{
            display: block;
        }
    &:hover .dis{
        display: none;
    }
}
.ms-btn{
        border: none;
        text-transform: uppercase;
        font-size: 12px;
        padding: 10px 20px;
        margin-right: 14px;
        position: relative;
        &:hover .line{
            display: none;
        }
       
    }
.ms-btn-secondary{
    background-color: $brand-primary;
    color: white;
}  

.line{
        padding: 0 8px;
        font-size: 20px;
        position: absolute;
        top: 2px;
        right: 30px;
    }
    
.map{
    position: relative;
    .dot-1{
        position: absolute;
        left: 22%;
        top: 40%;
    }
    .dot-2{
        position: absolute;
        left: 50%;
        top: 30%;
    }
    .dot-3{
        position: absolute;
        right: 14%;
        bottom: 27%;
    }
    .post-it{
        width: 200px;
        height: 60px;
        background-image: url(../assets/img/h1-contact-rev-03.png);
        background-size: cover;
        padding-left: 10px;
        padding-top: 8px;
        position: absolute;
        left: 22%;
        top: 49%;
        h5{
            font-size: 18px;
        }
    }
}

input, textarea{
    width: 100%;
    border: none;
    background-color: transparent;
    border-bottom: 1px solid lightgray;
    
}

</style>