<script>

export default{
    name:"ServiceProvide",
}

</script>

<template>
<section>
    <div class="column-left">
        <div class="card">
            <h4>Graphic Design</h4>
            <p>Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness.</p>
            <div class="box-img">
                <img src="../../assets/img/home-6-service-image-01.png" alt="">
            </div>
        </div>
        <div class="card">
            <div class="box-img">
                <img src="../../assets/img/home-6-service-image-03.png" alt="">
            </div>
            <h4>Idea Discussion</h4>
            <p>Get teamed up with the specialists who work and teach coding for years at famous universities.</p>
        </div>
    </div>
    <div class="column-center">
        <div class="card">
            <h4>Business Administration</h4>
            <p>Learners are encouraged to study the mechanism and structure of system administration.</p>
            <div class="box-img">
                <img src="../../assets/img/home-6-service-image-02.png" alt="">
            </div>
        </div>
        <div class="card">
            <div class="box-img">
                <img src="../../assets/img/home-6-service-image-04.png" alt="">            
            </div>
            <h4>Web Development</h4>
            <p>Learn to start building a webpage from scratch. You decide your own pace, course and speed.</p>
        </div>
    </div>
    <div class="column-right">
        <span class="color-grey">TOGETHER WE CAN CREATE</span>
        <h2>Services We <span>Can Provide</span> For My Clients.</h2>
        <ul>
            <li>
                <i class="fa-solid fa-check"></i>
                <span>Select & customize courses to your preferences</span>
            </li>
            <li>
                <i class="fa-solid fa-check"></i>
                <span>Change the tutor and make arrangements</span>
            </li>
            <li>
                <i class="fa-solid fa-check"></i>
                <span>Participate in events to join others</span>
            </li>
            <li>
                <i class="fa-solid fa-check"></i>
                <span>Get the desired certificate delivered at house</span>
            </li>
        </ul>
        <button class="color-white">Get started for free</button>
    </div>
</section>

</template>

<style lang="scss" scoped>
@use "../../styles/partials/mixins.scss" as * ;
@use "../../styles/partials/variables.scss" as * ;

section{
    @include flex(row,center,start);
    padding: 0 2rem;
    background-color:whitesmoke;
    text-align: left;
}

div.column-left{
    width: 25%;
}
div.column-center{
    width: 25%;
    margin: 0 1rem;
    padding-top: 50px;
}
div.column-right{
    width: 50%;
    align-self: center;

    &>:first-child{
        font-size: 1.5rem;
    }

    h2{
        padding: 2rem 0;
        font-size: 3.3rem;

        span{
            color: $in-hover;
        }
    }

    i{
        color:$in-hover;
        padding-right: 1rem;
    }

    li{
        padding-bottom: 1rem;
    }

    button{
        background-color: $in-hover;
        font-weight: bold;
    }
}

div.card{
    border-radius: 5px;
    background-color: white;
    margin: 1rem;

    h4{
        padding:2rem 0 1rem;
        padding-left: 1.5rem;
        font-size: 1.3rem;
    }

    p{
        padding-bottom: 1rem;
        padding-left: 1.5rem;
    }

    .box-img{
        height: 200px;
        width: 100%;

        img{
            width: 100%;
            height: 100%;
            display: block;
            object-fit: contain;
        }
    }
}



</style>