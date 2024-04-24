<script>
    export default{
    name: "MainCreative",

    }

</script>

<template>
    <section class="creative">
        <div class="btn-radious">
            <i class="fa-solid fa-arrow-up-long"></i>
        </div>
        <div class="container-page py-5 d-flex">
            <div class="col-6 py-5">
                <h4>Creative Leader<span class="brand-dot">.</span></h4>
                <div class="line-70 "></div>
                <p class="gray-text pt-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam officia odio quas suscipit perferendis vitae, culpa natus voluptas molestias quod doloremque eos officiis nemo quasi reprehenderit possimus corporis ut praesentium.</p>
                <div class="more pb-4">read more</div>
            </div>
            <div class="col-6 py-5">
                <div class="d-flex justify-content-between align-items-center">
                    <h6>Mentorship</h6>
                    <div>78%</div>
                </div>
                <div class="line-gray mb-4">
                    <div class="line-brand"></div>
                </div>
                <div class="d-flex justify-content-between align-items-center">
                    <h6>Education</h6>
                    <div>95%</div>
                </div>
                <div class="line-gray mb-4">
                    <div class="line-brand w1"></div>
                </div>
                <div class="d-flex justify-content-between align-items-center">
                    <h6>Learning</h6>
                    <div>65%</div>
                </div>
                <div class="line-gray mb-4">
                    <div class="line-brand w2"></div>
                </div>
                <div class="d-flex justify-content-between align-items-center">
                    <h6>Motivation</h6>
                    <div>83%</div>
                </div>
                <div class="line-gray">
                    <div class="line-brand w3"></div>
                </div>
                
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;
section{
    position: relative;
    background-color: white;
}

h4{
    font-size: 32px;
}
h6{
    font-size: 22px;
}

.line-70{
    width: 50px !important;
}

.line-gray{
    border-bottom: 1px solid #E1E1E1;
    position: relative;
}
.line-brand{
    border: 1px solid $brand-primary;
    width: 78%;
    position: absolute;
    bottom: -1px;
    left: 0;
    &.w1{
        width: 95%;
    }
    &.w2{
        width: 65%;
    }
    &.w3{
        width: 83%;
    }
}

.btn-radious{
    top: 40%
}

</style>