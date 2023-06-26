<script>

export default{
    name:"MainJumbotrone",
}

</script>

<template>
    <section>
        <h1>Learn At Your Own Pace!</h1>
        <p>Get teamed up with people of the same will.</p>
        <button>Get started for free</button>
        <div class="container">
            <img src="../assets/img/home-6-hero-left-person.png" alt="person">
            <img src="../assets/img/home-6-hero-right-person.png" alt="person" id="person-right">
            <div class="box-video">
            
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>
@use "../styles/partials/mixins.scss" as *;

section{
    text-align: center;
    background-color: blue;
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
}


</style>