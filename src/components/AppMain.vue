<script> 
import MainSpecialties from "./MainSpecialties.vue"
import MainFounder from "./MainFounder.vue"
import MainEvents from "./MainEvents.vue"
import MainCreative from "./MainCreative.vue"
import MainNews from "./MainNews.vue"
import MainTestimonials from "./MainTestimonials.vue"
import MainGallery from "./MainGallery.vue"

export default{
    name: "AppMain",
    components: {
        MainSpecialties,
        MainFounder,
        MainEvents,
        MainCreative,
        MainNews,
        MainTestimonials,
        MainGallery,

    },
        
}
</script>

<template>
    <MainSpecialties></MainSpecialties>
    <MainFounder></MainFounder>
    <MainEvents></MainEvents>
    <MainCreative></MainCreative>
    <MainNews></MainNews>
    <MainTestimonials></MainTestimonials>
    <MainGallery></MainGallery>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

</style>