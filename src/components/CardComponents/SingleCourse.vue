<script>

export default{
    name:"SingleCourse",

    props:{
        price: String,
        name :String,
        number_lessons :String,
        number_students :String,
        img : String
    },

    methods :{
        getImge(img){
            return new URL (`http://localhost:5173/src/assets/img/${img}`)
        }
    }

}

</script>

<template>
    <div class="card">
        <div class="box-img">
            <img :src="getImge(img)" alt="course img">
        </div>
        <div class="box-info">
            <span>{{ price }}</span>
            <h4>{{ name }}</h4>
            <i class="fa-solid fa-file-lines color-grey"></i>
            <span class="color-grey">{{ number_lessons }}</span>
            <i class="fa-solid fa-user color-grey"></i>
            <span class="color-grey ">{{ number_students }}</span>
        </div>
    </div>

</template>

<style lang="scss" scoped>
@use "../../styles/partials/mixins.scss" as *;
@use "../../styles/partials/variables.scss" as*;

.card{
    @include flex(row,start,start);
    width: calc(50% - 4rem);
    margin: 1rem;
}

.box-img{
    height: 200px;
    width: 200px;
    padding: 1rem;

    img{
        height: 100%;
        width: 100%;
        display: block;
        object-fit: cover;
        border-radius: 50%;
    }
}
.box-info{
    text-align: start;
    width: 60%;
    align-self: center;

    >*{
        padding: 0.5rem;
    }

    &>:first-child{
        color: $in-hover;
        font-weight: bold;
        font-size: 1.5rem;
    }

    h4{
        font-size: 1.3rem;
    }

    i{
        font-size: 0.8rem;
    }
}


</style>