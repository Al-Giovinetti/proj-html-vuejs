<script>
import MainJumbotrone from "./MainChild/MainJumbotrone.vue"
import ServiceProvide from "./MainChild/ServiceProvide.vue"

export default{
    name:"AppMain",

    components:{
        MainJumbotrone,
        ServiceProvide,
    }
}

</script>

<template>
<main>
    <MainJumbotrone />
    <ServiceProvide />
</main>

</template>

<style lang="scss" scoped>

</style>