<script>
import img1 from './../assets/img/rev-slider-main-home-img-03.jpg'
import img2 from './../assets/img/rev-slider-main-home-img-02.png'

export default{
name: 'AppHero',
    data(){
        return {
            heros: [img1, img2],
            isActive: 0,
        }
        
    },
    methods: {
        getImage(index){
            this.isActive= index;
            return this.heros[this.isActive]
           
            
        },
        showNext(){
            if (this.isActive < this.heros.length -1){
                this.isActive++;
            } else {
                this.isActive = 0;
            }
            
        },

        showPrevious(){
            if (this.isActive > 0){
                this.isActive--
            } else {
                this.isActive = this.heros.length - 1;
            }
        },

    }

}
</script>

<template>
    <section>
        <div class="left" @click="showPrevious">    
            <i class="fa-solid fa-arrow-left-long"></i>
        </div>
        <img :src="heros[isActive]" alt="">
        <div class="right" @click="showNext">
            <i class="fa-solid fa-arrow-right-long"></i>
        </div>
        <div class="hero-text col-4">
            <h1>Our Team<span>.</span></h1>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Totam consequuntur reiciendis blanditiis exercitationem, est vero.</p>
            <div>
                <button class="ms-btn ms-btn-primary">read more <span class="line">|</span><i class="ps-3 fa-solid fa-arrow-right-long"></i></button>
                <button class="ms-btn ms-btn-secondary">purchase<span class="line">|</span><i class="ps-3 fa-solid fa-arrow-right-long"></i></button>
            </div>
        </div>
    </section>
  
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;
img{
    width: 100%;
    height: 880px;
    object-fit: cover;
    position: absolute;
    top: -60px;
    right: 0;
}
section{
    .hero-text{
        position: absolute;
        left: 300px;
        top: 40%;
        z-index: 4;
        h1 {
            font-size: 70px;
            span{
                color: $brand-primary;
            }
        }
    }
    .left{
        font-size: 30px;
        position: absolute;
        top: 50%;
        left: 40px;
        z-index: 2;
        cursor: pointer;
    }
    .right{
        font-size: 30px;
        position: absolute;
        top: 50%;
        right: 40px;
        z-index: 2;
        cursor: pointer;
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
    
    .ms-btn-primary{
        background-color: white;

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
    p{
    color: $color-secondary;
    }  
}


</style>
