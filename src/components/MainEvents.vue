<script>
    export default{
    name: "MainEvents",

    }

</script>

<template>
    <section class="events">
        <div class="container-fluid">
            <div class="btn-radious">
                <i class="fa-solid fa-arrow-up-long"></i>
            </div>
            <div class="container-page">
                <div class="card col-5">
                    <div class="card-header p-3 px-4">
                        <h4>Upcoming Events</h4>
                    </div>
                    <ul class="list-group list-group-flush">
                        <li class="list-group-item d-flex">
                            <div class="data">
                                <div>07</div>
                                <div><small>Jan 2022</small></div>
                            </div>
                            <div class="info">
                                <h6>Melbourne Coaching</h6>
                                <div class="d-flex"><i class="fa-regular fa-clock brand-color pe-2"></i><p class="gray-text">9:00 am - 5:00 pm, Jan 7, 2022</p></div>
                                <div class="d-flex"><i class="fa-solid fa-location-dot brand-color pe-2"></i> <p class="gray-text">Cambridge, MA 02138, USA</p></div>
                                <div class="more pb-4">read more</div>
                            </div>
                        </li>
                        <li class="list-group-item d-flex">
                            <div class="data">
                                <div>11</div>
                                <div><small>Jan 2022</small></div>
                            </div>
                            <div class="info">
                                <h6>New York Coaching</h6>
                                <div class="d-flex"><i class="fa-regular fa-clock brand-color pe-2"></i><p class="gray-text">9:00 am - 5:00 pm, Jan 7, 2022</p></div>
                                <div class="d-flex"><i class="fa-solid fa-location-dot brand-color pe-2"></i> <p class="gray-text">Cambridge, MA 02138, USA</p></div>
                                <div class="more pb-4">read more</div>
                            </div>
                        </li>
                        <li class="list-group-item d-flex">
                            <div class="data">
                                <div>21</div>
                                <div><small>Jan 2022</small></div>
                            </div>
                            <div class="info">
                                <h6>London Coaching</h6>
                                <div class="d-flex"><i class="fa-regular fa-clock brand-color pe-2"></i><p class="gray-text">9:00 am - 5:00 pm, Jan 7, 2022</p></div>
                                <div class="d-flex"><i class="fa-solid fa-location-dot brand-color pe-2"></i> <p class="gray-text">Cambridge, MA 02138, USA</p></div>
                                <div class="more pb-4">read more</div>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;
.container-page{
    position: relative;
    .col-5{
        position: absolute;
        left: 0;
        top: 100px;
    }
}
.container-fluid{
    position: relative;
    background-image: url(../assets/img/h1-img-09.jpg);
    background-size: cover;
    height: 840px;
    .btn-radious{
        top: 50%;
        right: 20px;
    }
    .data{
        text-align: center;
        background-color: $brand-primary;
        color: white;
        padding: 4px 6px;
        margin-right: 16px;
        height: 30%;
    }
    
    .info{
        p{
            font-size: 12px;
        }
    }
    h6{
        font-size: 24px;
    }

    h4{
        font-size: 30px;
    }
    .card-header{
        background-color: #F9F9F9;
    }
    li{
        background-color: #F9F9F9;
        cursor: pointer;
        &:hover{
            background-color: white;
            h6{
                color: $brand-primary;
            }
        }
    }
}

</style>