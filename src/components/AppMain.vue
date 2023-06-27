<script>
import MainJumbotrone from "./MainChild/MainJumbotrone.vue"
import ServiceProvide from "./MainChild/ServiceProvide.vue"
import CoursesList from "./MainChild/CoursesList.vue"

export default{
    name:"AppMain",

    components:{
        MainJumbotrone,
        ServiceProvide,
       CoursesList,
    }
}

</script>

<template>
<main>
    <MainJumbotrone />
    <ServiceProvide />
    <CoursesList />
</main>

</template>

<style lang="scss" scoped>

</style>