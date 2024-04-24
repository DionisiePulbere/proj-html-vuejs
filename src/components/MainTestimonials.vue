
<script>
import img1 from './../assets/img/h3-img-04.png'
import img2 from './../assets/img/h3-img-07.png'
import img3 from './../assets/img/h3-img-08.png'

    export default{
        name: "MainTestimonials",
        data(){
            return {
                blogs: [
                    {
                        image:img1,
                        name:"Cynthia Clark",
                        number: "01",
                        class: "jcs"
                    },
                    {
                        image:img2,
                        name:"Mulan Tsou",
                        number: "02",
                        class: "jcc"
                    },
                    {
                        image:img3,
                        name:"Ellan W. Gentry",
                        number: "03",
                        class: "jce"
                    }
                ],
                isActive: 0,
                class: "",
            }
        },
        methods: {
            getImage(index){
                this.isActive= index;
                return this.blogs[this.isActive]
            
                
            },
            showNext(){
                if (this.isActive < this.blogs.length -1){
                    this.isActive++;
                } else {
                    this.isActive = 0;
                }
                
            },

            showPrevious(){
                if (this.isActive > 0){
                    this.isActive--
                } else {
                    this.isActive = this.blogs.length - 1;
                }
            },
            

        },
        computed: {
            showClass(){
                this.class = this.blogs[this.isActive].class
                return this.class

            }
            
        }

    }

</script>

<template>
    <section class="testimonials">
        <div class="container-fluid">
            <div class="btn-radious">
                <i class="fa-solid fa-arrow-up-long"></i>
            </div>
            <h1>Testimonials.</h1>
            <div class="left" @click="showPrevious">    
                <i class="fa-solid fa-arrow-left-long"></i>
            </div>
            <div class="right" @click="showNext">
                <i class="fa-solid fa-arrow-right-long"></i>
            </div>
            <div class="info col-4 text-center">
                <img :src="blogs[isActive].image" alt="">
                <div class="text-white py-3">{{blogs[isActive].name}}</div>
                <p class="text-white">"Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dolorum quaerat, placeat quam ea fuga, veritatis nisi est commodi sed"</p>
                <div class="d-flex justify-content-center align-items-center">
                    <div class="text-white">{{ blogs[isActive].number }}</div>
                    <div class="line-100 mx-2" :class="class">
                        <div class="line-33"></div>
                    </div>
                    <div class="text-white">03</div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;
section{
    position: relative;
    height: 500px;
    background-color: rgba(0, 0, 0, 0.9);
}
h1{
    font-size: 240px;
    text-align: center;
    position: absolute;
    top: 0;
    left: 50%;
    transform: translateX(-50%);
    z-index: -1;
}

img{
    width: 80px;
}

.info{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

.line-100{
    width: 90px;
    border-bottom: 1px solid lightgray;
    display: flex;
}
.jcs{
    justify-content: start;
}
.jcc{
    justify-content: center;
}
.jce{
    justify-content: end;
}


.line-33{
    width: calc(100% / 3);
    border-bottom: 1px solid white;
    
}
.left{
    color: white;
    font-size: 30px;
    position: absolute;
    top: 50%;
    left: 40px;
    z-index: 2;
    cursor: pointer;
}
.right{
    color: white;
    font-size: 30px;
    position: absolute;
    top: 50%;
    right: 40px;
    z-index: 2;
    cursor: pointer;
}
.btn-radious{
    top: 20%;
}
</style>