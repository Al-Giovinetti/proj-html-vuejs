<script>


export default{
    name:"SingleNews",

    props:{
        news:Object
    }

}

</script>

<template>
    <div class="card">
        <img :src="news.img" alt="aaaaaa">
        <span class="color-grey">{{ news.subject }}</span>
        <p>{{ news.title }}</p>
        <i class="fa-regular fa-calendar color-grey"></i>
        <span class="color-grey">{{ news.date }}</span>
        <i class="fa-regular fa-eye color-grey"></i>
        <span class="color-grey">{{  news.views}}</span>
    </div>

</template>

<style lang="scss" scoped>
    div.card{
        width: calc(100% / 3 - 4rem);
        margin: 2rem;

        img{
            width: 100%;
            border-radius: 10px;
            padding-bottom: 2rem;
        }

        p{
            font-weight: bold;
            font-size: 1.5rem;
            padding: 1.5rem 0;
        }

        i{
            padding: 0.5rem;
        }
    }


</style>