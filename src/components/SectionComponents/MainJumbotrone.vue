<script>

export default{
    name:"MainJumbotrone",
}

</script>

<template>
    <section class="jumbotrone">
        <h1 class="color-white">Learn At Your Own Pace!</h1>
        <p class="color-grey">Get teamed up with people of the same will.</p>
        <button class="color-white" id="started-free">Get started for free</button>
        <div class="container">
            <img src="../../assets/img/home-6-hero-left-person.png" alt="person">
            <img src="../../assets/img/home-6-hero-right-person.png" alt="person" id="person-right">
            <div class="box-video">
                <img src="../../assets/img/home-6-hero-poster-final.jpg" alt="page whit grafic">
                <img src="../../assets/img/icon-youtube-play.png" alt="youtube logo">
            </div>
        </div>
    </section>
    <section>
        <p>aaaaaaaaaa</p>
        <span>aaa</span>
        <span>aaa</span>
        <div class="numbers">
            <div>
                <p>1000</p>
                <span>aaaaaa</span>
            </div>
            <div>
                <p>1000</p>
                <span>aaaaaa</span>
            </div>
            <div>
                <p>1000</p>
                <span>aaaaaa</span>
            </div>
            <div>
                <p>1000</p>
                <span>aaaaaa</span>
            </div>
        </div>

    </section >

</template>

<style lang="scss" scoped>
@use "../../styles/partials/mixins.scss" as *;
@use "../../styles/partials/variables.scss" as*;

h1{
    font-size: 3rem;
    padding-top:2rem;
    padding-bottom: 1rem;
}



#started-free{
    position: relative;
    top: 30px;
    background-color: $in-hover;
}

section.jumbotrone{
    text-align: center;
    background-color:$bg-page-top;
    margin-bottom: 180px
}
div.container{
    @include flex(row,space-between,center);
    position: relative;
    top: 100px;

    >img{
        position: relative;
        align-self: flex-end;
        right: 60px;
    }
}

img#person-right{
            position: relative;
            top:50px;
}
div.box-video{
    min-width: 55%;
    height: 90%;
    border-radius: 20px;
    position: absolute;
    left: 50%; top:50%;
    transform: translate(-50%,-50%);
    background-color: white;
    padding: 1rem;

    img:first-child{
        width: 100%;
        height: 100%;
        display: block;
        object-fit: cover;
    }

    img:nth-child(2){
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%,-50%);
        height: 70px;
    }
}

div.numbers{
    @include flex(row,space-evenly,center);
}



</style>