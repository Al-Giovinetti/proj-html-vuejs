<script>

export default{
    name:"ServiceProvide",
}

</script>

<template>
<section>
    <div class="column-left">
        <div class="card">
            <span>aaaaaaa</span>
            <p>aaaaaaa</p>
            <div class="box-img">
                <img src="../../assets/img/home-6-service-image-01.png" alt="">
            </div>
        </div>
        <div class="card">
            <div class="box-img">
                <img src="../../assets/img/home-6-service-image-03.png" alt="">
            </div>
            <span>aaaaaaa</span>
            <p>aaaaaaa</p>
        </div>
    </div>
    <div class="column-center">
        <div class="card">
            <span>aaaaaaa</span>
            <p>aaaaaaa</p>
            <div class="box-img">
                <img src="../../assets/img/home-6-service-image-02.png" alt="">
            </div>
        </div>
        <div class="card">
            <div class="box-img">
                <img src="../../assets/img/home-6-service-image-04.png" alt="">            
            </div>
            <span>aaaaaaa</span>
            <p>aaaaaaa</p>
        </div>
    </div>
    <div class="column-right">
        <span>aaaaa</span>
        <p>aaaaaaa</p>
        <ul>
            <li>aaaa</li>
            <li>aaa</li>
            <li>aaa</li>
            <li>aaa</li>
        </ul>
        <button>aaaaaaa</button>
    </div>
</section>

</template>

<style lang="scss" scoped>
@use "../../styles/partials/mixins.scss" as * ;

section{
    @include flex(row,center,start);
    text-align: center;
    padding: 0 2rem;
}

div.column-left{
    width: 25%;
    border: 1px solid black;
}
div.column-center{
    width: 25%;
    margin: 0 2em;
    border: 1px solid black;
    padding-top: 50px;
}
div.column-right{
    width: 50%;
    border: 1px solid black;
    align-self: center;
}

div.card{
    border: 1px solid rgb(245, 12, 12);
    margin: 1rem;

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