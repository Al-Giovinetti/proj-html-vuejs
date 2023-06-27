<script>
import SingleCourse from "../CardComponents/SingleCourse.vue"

export default{
    name:"CoursesList",

    components:{
        SingleCourse,
    },

    data(){
        return{
            Courses : [
                {
                    price: "Free",
                    name: "Personal Finance: Financial Security Thinking & Principles",
                    number_lessons : "2 Lessons",
                    number_students :"260 Students",
                    img:"stock-full-hd-05-480x298.jpg"
                },
                {
                    price: "$40",
                    name: "Learning to Write as a Professional Author",
                    number_lessons : "20 Lesson",
                    number_students :"69 Students",
                    img:"course-02-480x298.jpg"
                },
                {
                    price: "Free",
                    name: "Customer-centric Info-Tech Strategies",
                    number_lessons : "24 Lessons",
                    number_students :" 927 Students",
                    img:"stock-full-hd-03-480x298.jpg"
                },
                {
                    price: "$19",
                    name: "Open Programming Courses for Everyone: Python",
                    number_lessons : "17 Lessons",
                    number_students :"66 Students",
                    img:"stock-full-hd-04-480x298.jpg"
                },
                {
                    price: "$26",
                    name: "Academic Listening and Note-taking",
                    number_lessons : "14 Lessons",
                    number_students :"68 Students",
                    img:"stock-full-hd-06-480x298.jpg"
                },
                {
                    price: "Free",
                    name: "Master jQuery in a Short Period of Time",
                    number_lessons : "6 Lessons",
                    number_students :"51 Students",
                    img:"course-featured-image-01-480x298.jpg",
                },
            ]
        }
    }
}

</script>

<template>
    <section>
        <p class="color-grey">CHOOSE A COURSE TO GET STARTED</p>
        <h2>Latest Featured <span>Courses</span></h2>
        <div class="container">
            <SingleCourse v-for="course in Courses" 
            :price = course.price
            :name = course.name
            :number_lessons = course.number_lessons
            :number_students = course.number_students
            :img = course.img />
        </div>
        <button class="color-white">View all courses</button>
    </section>
</template>

<style lang="scss" scoped>
@use "../../styles/partials/variables.scss" as*;

section:not(div.container){
    text-align: center;
    background-color: rgb(239, 239, 239);
    padding-top: 3rem;

    h2{
        padding: 2rem;
        font-size: 2rem;
    }

    h2>span{
        color: $in-hover;
    }
}
.container{
    display: flex;
    flex-wrap: wrap;
}

button{
    background-color: $in-hover;
    margin-bottom: 2rem;
}

</style>