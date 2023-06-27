<script>
import MainJumbotrone from "./SectionComponents/MainJumbotrone.vue"
import ServiceProvide from "./SectionComponents/ServiceProvide.vue"
import CoursesList from "./SectionComponents/CoursesList.vue"
import TalkAbout from "./SectionComponents/TalkAbout.vue"

export default{
    name:"AppMain",

    components:{
        MainJumbotrone,
        ServiceProvide,
        CoursesList,
        TalkAbout,
    }
}

</script>

<template>
<main>
    <MainJumbotrone />
    <ServiceProvide />
    <CoursesList />
    <TalkAbout />
</main>

</template>

<style lang="scss" scoped>

</style>