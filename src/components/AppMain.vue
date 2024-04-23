<script> 
import MainSpecialties from "./MainSpecialties.vue"
import MainFounder from "./MainFounder.vue"
import MainEvents from "./MainEvents.vue"
import MainCreative from "./MainCreative.vue"

export default{
    name: "AppMain",
    components: {
        MainSpecialties,
        MainFounder,
        MainEvents,
        MainCreative,
    },
        
}
</script>

<template>
    <MainSpecialties></MainSpecialties>
    <MainFounder></MainFounder>
    <MainEvents></MainEvents>
    <MainCreative></MainCreative>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

</style>