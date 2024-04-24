<script>
    export default{
    name: "MainNews",

    }

</script>

<template>
    <section class="news py-5">
        <div class="container-page py-5">
            <div class="text-center">
                <h2>Latest news<span class="brand-dot">.</span></h2>
                <p class="gray-text">Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
                <div class="line-70 mb-5"></div>
            </div>
            <div class="d-flex p-2">
                <div class="col-4">
                    <div class="photo me-3">
                        <div class="top">
                            <img src="../assets/img/h1-blog-img-02.jpg" alt="">
                        </div>
                        <div class="bottom">
                            <img src="../assets/img/h1-blog-img-03.jpg" alt="">
                        </div>
                        <div class="ms-badge d-flex"><i class="fa-solid fa-tag me-2"></i> Business, Leading</div>
                    </div>
                    <div class="info mt-4">
                        <div class="date d-flex">
                            <p class="gray-text"><i class="fa-regular fa-clock"></i> May 5, 2019 <i class="fa-regular fa-user"></i> Amanda Doe</p>
                        </div>
                        <h3>Next Investment</h3>
                        <p class="gray-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam neque cumque cupiditate ...</p>
                        <div class="more">read more</div>
                    </div>
                </div>
                <div class="col-4 me-3">
                    <div class="photo">
                        <div class="top">
                            <img src="../assets/img/h1-blog-img-03.jpg" alt="">
                        </div>
                        <div class="bottom">
                            <img src="../assets/img/h1-blog-img-04.jpg" alt="">
                        </div>
                        <div class="ms-badge d-flex"><i class="fa-solid fa-tag me-2"></i> Business, Leading</div>
                    </div>
                    <div class="info mt-4">
                        <div class="date d-flex">
                            <p class="gray-text"><i class="fa-regular fa-clock"></i> May 5, 2019 <i class="fa-regular fa-user"></i> Amanda Doe</p>
                        </div>
                        <h3>Team Building</h3>
                        <p class="gray-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam neque cumque cupiditate ...</p>
                        <div class="more">read more</div>
                    </div>
                </div>
                <div class="col-4 ">
                    <div class="photo ">
                        <div class="top">
                            <img src="../assets/img/h1-blog-img-04.jpg" alt="">
                        </div>
                        <div class="bottom">
                            <img src="../assets/img/h1-blog-img-01.jpg" alt="">
                        </div>
                        <div class="ms-badge d-flex"><i class="fa-solid fa-tag me-2"></i> Business, Leading</div>
                    </div>
                    <div class="info mt-4">
                        <div class="date d-flex">
                            <p class="gray-text"><i class="fa-regular fa-clock"></i> May 5, 2019 <i class="fa-regular fa-user"></i> Amanda Doe</p>
                        </div>
                        <h3>New Business Day</h3>
                        <p class="gray-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam neque cumque cupiditate ...</p>
                        <div class="more">read more</div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;
section{
    position: relative;
}

.line-70{
    margin: 0 auto;
}
.photo{
    height: 200px;
    position: relative;
}
.top{
    height: 40%;
    overflow: hidden;
    img{
        width: 100%;
    }
}

.bottom{
    height: 60%;
    overflow: hidden;
    img{
        width: 100%;
        object-position: 0 -80px;
    }
}

.ms-badge{
    background-color: $brand-primary;
    padding: 10px;
    color: white;
    font-size: 12px;
    font-weight: 100;
    position: absolute;
    bottom: -12px;
    right: 16px;
    align-items: center;
}

.date{
    font-size: 14px;
    i{
        color: $brand-primary;
    }
}

</style>