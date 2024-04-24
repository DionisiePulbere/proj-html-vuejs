<script> 
import MainSpecialties from "./MainSpecialties.vue"
import MainFounder from "./MainFounder.vue"
import MainEvents from "./MainEvents.vue"
import MainCreative from "./MainCreative.vue"
import MainNews from "./MainNews.vue"
import MainTestimonials from "./MainTestimonials.vue"

export default{
    name: "AppMain",
    components: {
        MainSpecialties,
        MainFounder,
        MainEvents,
        MainCreative,
        MainNews,
        MainTestimonials,
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
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

</style>