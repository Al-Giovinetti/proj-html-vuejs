<script>

export default{
    name:"MainJumbotrone",
}

</script>

<template>
    <section class="jumbotrone">
        <h1>Learn At Your Own Pace!</h1>
        <p>Get teamed up with people of the same will.</p>
        <button>Get started for free</button>
        <div class="container">
            <img src="../../assets/img/home-6-hero-left-person.png" alt="person">
            <img src="../../assets/img/home-6-hero-right-person.png" alt="person" id="person-right">
            <div class="box-video">
                <img src="../../assets/img/home-6-hero-poster-final.jpg" alt="screen">
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

section.jumbotrone{
    text-align: center;
    background-color:$bg-primary;
    margin-bottom: 180px
}
div.container{
    @include flex(row,space-between,center);
    position: relative;
    top: 100px;
    border:1px solid black;

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
    border: 1px solid black;
    border-radius: 20px;
    position: absolute;
    left: 50%; top:50%;
    transform: translate(-50%,-50%);
    background-color: white;
    padding: 1rem;

    img{
        width: 100%;
        height: 100%;
        display: block;
        object-fit: cover;
    }
}

section{
    text-align: center
}
div.numbers{
    @include flex(row,space-evenly,center);
}



</style>