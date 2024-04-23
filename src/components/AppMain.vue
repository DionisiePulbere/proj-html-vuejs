<script> 
import MainSpecialties from "./MainSpecialties.vue"
import MainFounder from "./MainFounder.vue"
import MainEvents from "./MainEvents.vue"

export default{
    name: "AppMain",
    components: {
        MainSpecialties,
        MainFounder,
        MainEvents,
    },
        
}
</script>

<template>
    <MainSpecialties></MainSpecialties>
    <MainFounder></MainFounder>
    <MainEvents></MainEvents>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

</style>