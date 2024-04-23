<script> 
import MainSpecialties from "./MainSpecialties.vue"
import MainFounder from "./MainFounder.vue"

export default{
    name: "AppMain",
    components: {
        MainSpecialties,
        MainFounder,
    },
        
}
</script>

<template>
  <MainSpecialties></MainSpecialties>
  <MainFounder></MainFounder>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

</style>