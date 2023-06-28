<script>
import SingleNews from "../CardComponents/SingleNews.vue"


export default{
    name:"OursNews",

    components:{
        SingleNews,   
    },

    data(){
        return{
            news:[
                {
                img:"https://st2.depositphotos.com/1000423/7385/i/600/depositphotos_73854849-stock-photo-office-work-moments.jpg",
                subject:"BUSINESS",
                title:"Ten Benefits Of Rentals That May Change Your Perspective",
                date:" Dec 28, 2020",
                views:" 2,621 views"
                },
                {
                img:"https://img.freepik.com/premium-photo/young-female-manager-her-workplace-with-laptop-discussing-work-moments-with-her-pregnant-colleague-office-modern-pregnant-office-worker_173815-41222.jpg",
                subject:"BUSINESS",
                title:"10 Things Successful Mompreneurs Do Differente",
                date:" Dec 28, 2020",
                views:" 2,341 views"
                },
                {
                img:"https://st4.depositphotos.com/2251265/26614/i/600/depositphotos_266146836-stock-photo-working-moments-group-of-young.jpg",
                subject:"BUSINESS",
                title:"How Stay Calm from the First Time.",
                date:" Dec 28, 2020",
                views:"1,723 views"
                }
            ]
        }
    }
}

</script>

<template>
    <section>
        <p class="color-grey">ENJOY READING ON MAXCOACH</p>
        <h2>Latest on <span>Our Blogs</span></h2>
        <div class="container">
            <SingleNews  v-for="n in news"
            :news = "n"/>
        </div>
    </section>


</template>

<style lang="scss" scoped>
@use "../../styles/partials/mixins.scss" as*;
@use "../../styles/partials/variables.scss" as*;
section>*:not(div.container){
    text-align: center;
    padding-top: 3rem
}
div.container{
    @include flex(row,space-around,start);

}

h2{
    font-size: 2.5rem;
    span{
        color:$in-hover
    }
}


</style>