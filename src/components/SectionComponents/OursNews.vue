<script>
import SingleNews from "../CardComponents/SingleNews.vue"


export default{
    name:"OursNews",

    components:{
        SingleNews,
        
    }
}

</script>

<template>
    <section>
        <p>aaaaaaa</p>
        <h2>aaaaaaaa</h2>
        <div class="container">
            <SingleNews  v-for="n in 3"/>
        </div>
    </section>


</template>

<style lang="scss" scoped>
@use "../../styles/partials/mixins.scss" as*;

div.container{
    @include flex(row,space-around,start)
}


</style>