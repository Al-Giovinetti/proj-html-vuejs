<script>


export default{
    name:"TalkAbout",

    data(){
        return{
            
        }
    }
}

</script>

<template>
    <section>
        <h2>Why People Talk About <span>MaxCoach</span>?</h2>
        <div class="d-flex testimonial">
            <div class="box-img">
                <img src="../../assets/img/testimonial-avata-02.jpg" alt="testimonial-1">
            </div>
            <div class="info-box">
                <p>I am free to learn at my own pace, follow my own schedule and choose the subject I like. Great study portal for people like me.</p>
                <span>MINA HOLLACE</span>
                <span class="color-grey">/Freelancer</span>
            </div>
        </div>
        <div class="d-flex clients">
            <div class="box-img">
                <img src="../../assets/img/client-logo-colored-01.png" alt="">
            </div>
            <div class="box-img">
                <img src="../../assets/img/client-logo-colored-02.png" alt="">
            </div>
            <div class="box-img">
                <img src="../../assets/img/client-logo-colored-03.png" alt="">
            </div>
            <div class="box-img">
                <img src="../../assets/img/client-logo-colored-04.png" alt="">
            </div>
            <div class="box-img">
                <img src="../../assets/img/client-logo-colored-05.png" alt="">
            </div>
            <div class="box-img">
                <img src="../../assets/img/client-logo-colored-06.png" alt="">
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>
@use "../../styles/partials/variables.scss" as*;


h2{
    text-align: center;
    font-size: 2.5rem;
    padding: 3rem;
    span{
        color:$in-hover
    }
}

div.testimonial{
    width: 70%;
    margin:auto;
    div.box-img{
        width: 200px;
        height: 200px;
    img{
        height: 100%;
        width: 100%;
        border-radius: 50%;
        object-fit: cover;
    }
    }

    div.info-box{
        align-self: center;
        width: 80%;
        padding: 3rem;

        p{
            font-size: 2.1rem;
        }

        span{
            display: block;
            padding-top: 1rem;
        }
    }
}

div.clients{
    display: flex;
    justify-content: space-around;
    .box-img{
        height: 100px;
        width: 100px;
    }

    img{
        width: 100%;
        height: 70px;
        object-fit: contain;
    }
}


</style>