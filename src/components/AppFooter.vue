<script>
    export default{
    name: "AppFooter",
        data(){
            return{
                footerList: [
                    {
                        title: "About",
                        text: "We created Everlead to effectively become the stepping stone towards meeting all your goals & achiving business success."
                    },
                    {
                        title: "Twitter",
                        content: [
                            {
                                icon: "fa-brands fa-twitter",
                                text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates praesentium inventore veritatis expedita"
                            },
                            {
                                icon: "fa-brands fa-twitter",
                                text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates praesentium inventore veritatis expedita"
                            }
                        ]

                    },
                    {
                        title: "Important link",
                        link: ["About me", "About us", "Language packs", "Become a coach", "Monthly events"]
                    },
                    {
                        title: "Contact me",
                        content:[
                            {
                                icon: "fa-solid fa-location-dot",
                                text: "457 BigBlue Street, NY 10013"
                            },
                            {
                                icon: "fa-solid fa-location-dot",
                                text: "(315) 5512-2579"
                            },
                            {
                                icon: "fa-solid fa-envelope",
                                text: "everlead@mikado.com"
                            }

                        ]
                    }
                ],
                socials: ["fa-brands fa-linkedin-in", "fa-brands fa-facebook-f", "fa-brands fa-twitter"]
            }
        }
    }

</script>

<template>
    <footer>
        <div class="black py-5">
            <div class="container-page d-flex py-5">
                <div v-for="list in footerList" class="col-3 mx-3">
                    <h2>{{list.title}}</h2>
                    <div class="line-70 mb-4"></div>
                    <ul v-if="list.text" >
                        <li>
                            <p class="gray-text">{{ list.text }}</p>
                        </li>
                        <li>
                             <div v-for="social in socials" class="d-flex social">
                                <i :class="social"></i>
                            </div>
                        </li>
                    </ul>
                    <ul v-else-if="list.link">
                        <li class="gray-text mb-1" v-for="link in list.link">{{ link }}
                        </li>
                        
                    </ul>
                    <ul v-else>
                        <li v-for="content in list.content">
                            <i :class="content.icon"></i>
                            <p class="gray-text">{{ content.text }}</p>
                        </li>
                    </ul>
                </div>
                <div class="d-flex sub">
                    <input class="subscribe" type="text" placeholder="Your Name"> 
                    <button>SUBSCRIBE</button>
                </div>
            </div>
        </div>
        <div class="red py-2">
            Copyright Boolean@Dionisie Pulbere
        </div>
        <div class="btn-radious">
            <i class="fa-solid fa-arrow-up-long"></i>
        </div>
    </footer>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

footer{
    position: relative;
}
.black{
    background-color: black;
    color: white;
}
.red{
    background-color: $brand-primary;
    color: white;
    font-weight: 100;
    text-align: center;
}

h2{
    font-size: 30px;
    color: white;
}

.social i{
    background-color: white;
    color: black;
    &:hover{
        background-color: $brand-primary;
        color: white;
    }
}

.line-70{
    width: 40px;
}

ul{
    padding: 0 !important;
}
li{
    display: flex;
    align-items: baseline;
    line-height: 24px;
   
    i{
        margin-right: 10px;
        color: $brand-primary;
    }
}

.sub{
    border-bottom: 1px solid white;
    position: absolute;
    right: 200px;
    top: 60%;
    input{
        background-color: black;
        border: none;
        color: white;
        &:focus-visible{
            outline: none;

        }
    }
    button{
        background-color: black;
        border: none;
        color: white;
    }
}

.btn-radious{
    bottom: 26px;

}



</style>