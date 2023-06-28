<script>

export default{
    name:"HelpLearn",
}

</script>

<template>
    <section>
        <p class="color-grey">WANNA TRANSFORM YOUR LIFE?</p>
        <h2>Glad to <span>Help You </span>Learn</h2>
        <div class="container">
            <div>
                <i class="fa-regular fa-flag"></i>
                <span>Idea Discussion</span>
                <p class="color-grey">Get teamed up with the specialists who work and teach coding for years at famous universities.</p>
            </div>
            <div>
                <i class="fa-solid fa-gear"></i>
                <span>Web Development</span>
                <p class="color-grey">Learn to start building a webpage from scratch. You decide your own pace, course and speed.</p>
            </div>
            <div>
                <i class="fa-regular fa-life-ring"></i>
                <span>System Administration</span>
                <p class="color-grey">Learners are encouraged to study the mechanism and structure of system administration.</p>
            </div>
            <div>
                <i class="fa-solid fa-desktop"></i>
                <span>Graphic Design</span>
                <p class="color-grey">Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness.</p>
            </div>
        </div>
        <img src="../../assets/img/home-6-services-image.png" alt="persons">
        <p>Start today for getting <span>Online Certification</span></p>
        <p>You can be your own guiding star with our help!</p>
        <button class="color-white">Get started now</button>
    </section>

</template>

<style lang="scss" scoped>
@use "../../styles/partials/mixins.scss" as * ;
@use "../../styles/partials/variables.scss" as*;


section:not(div.container){
    text-align: center;
    padding-top:3rem;

    h2{
        font-size: 3rem;
        padding: 2rem;
            span{
                color:$in-hover;
            }
    }
}

div.container{
    @include flex(row,space-around,start);

    div{
        @include flex(column,start,start);
        margin: 2rem;

        >*{
            padding-bottom: 1rem;
        }

        i{
            font-size: 4rem;
        }

        p{
            text-align: left;
            line-height: 20px;
        }

        span{
            font-weight: bold;
            font-size: 1.2rem;
        }
    }
}

img{
    width:90%;
    margin: auto;
    padding-bottom: 2rem;

    ~p{padding: 0.5rem;
        font-size: 1.5rem;
        font-weight: bold;

        >span{
        color: $in-hover;
    }
    }
}

button{
    margin: 2rem 0;
    background-color: $in-hover;
}
</style>