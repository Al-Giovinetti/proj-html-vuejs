<script>
import MainJumbotrone from "./SectionComponents/MainJumbotrone.vue"
import ServiceProvide from "./SectionComponents/ServiceProvide.vue"
import CoursesList from "./SectionComponents/CoursesList.vue"
import TalkAbout from "./SectionComponents/TalkAbout.vue"
import OursNews from "./SectionComponents/OursNews.vue"
import HelpLearn from "./SectionComponents/HelpLearn.vue"

export default{
    name:"AppMain",

    components:{
        MainJumbotrone,
        ServiceProvide,
        CoursesList,
        TalkAbout,
        OursNews,
        HelpLearn
    }
}

</script>

<template>
<main>
    <MainJumbotrone />
    <ServiceProvide />
    <CoursesList />
    <TalkAbout />
    <OursNews />
    <HelpLearn />

</main>

</template>

<style lang="scss" scoped>

</style>