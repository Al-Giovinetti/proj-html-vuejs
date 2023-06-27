<script>
import SingleCourse from "../CardComponents/SingleCourse.vue"

export default{
    name:"CoursesList",

    components:{
        SingleCourse,
    }
}

</script>

<template>
    <section>
        <p>aaaaaaaaa</p>
        <h2>aaaaaaaaaaaaaaaa</h2>
        <div class="container">
            <SingleCourse v-for="n in 6" />
        </div>
        <button>View all courses</button>
    </section>
</template>

<style lang="scss" scoped>

section:not(div.container){
    text-align: center;
}

.container{
    display: flex;
    flex-wrap: wrap;
}

</style>