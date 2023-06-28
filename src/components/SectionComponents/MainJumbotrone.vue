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
    <section class="sec-bottom">
        <div class="founder">
            <p>Let passion and determination be the guide along the way and develop at your own pace that's confortable </p>
            <span>FANNI MORENO</span>
            <span class="color-grey d-block">/Founder e CEO</span>
        </div>
        <div class="numbers">
            <div>
                <p>1926</p>
                <span class="color-grey">FINISHED SESSIONS</span>
            </div>
            <div>
                <p>3.092+</p>
                <span class="color-grey">ENROLLED LEARNERS</span>
            </div>
            <div>
                <p>200</p>
                <span class="color-grey">ONLINE INSTRUCTORS</span>
            </div>
            <div>
                <p>100%</p>
                <span class="color-grey">SATISFACTION RATE</span>
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
    overflow:hidden;

    img:first-child{
        width: 100%;
        height: 100%;
        display: block;
        object-fit: contain;
        padding: 1rem;
        transition: all 2s;

        &:hover{
            transform: scale(1.2);
        }
    }

    img:nth-child(2){
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%,-50%);
        height: 70px;
    }
}

.sec-bottom{
    background-color: whitesmoke;
    padding-top: 180px;
    text-align: center;
}

div.founder{
    margin: auto;
    width: 50%;

    p{
        padding-top: 50px;
        font-size: 2rem;
        font-weight: bold;
        line-height: 3rem;
        padding-bottom: 2rem;
    }

    span:not(.d-block){
        font-weight: bolder;
    }

    span.d-block{
    padding: 1rem 0 2rem
}
}

div.numbers{
    @include flex(row,space-evenly,center);
    padding-bottom: 3rem;

    p{
        color:$in-hover;
        font-size: 3rem;
        font-weight: bold;
    }

    span{
        font-weight: bold
    };
}



</style>