<script>

export default{
    name:"SingleCourse",

}

</script>

<template>
    <div class="card">
        <div class="box-img">
            <img src="" alt="aaaaaaa">
        </div>
        <div class="box-info">
            <span>aaaaaa</span>
            <h4>aaaaaaaaaa</h4>
            <span>1243</span>
            <span>aaaaa</span>
        </div>
    </div>

</template>

<style lang="scss" scoped>
@use "../../styles/partials/mixins.scss" as *;

.card{
    @include flex(row,start,start);
    width: 50%;
    border: 1px solid black;
}

.box-img{
    height: 200px;
    width: 200px;

    img{
        height: 100%;
        width: 100%;
        display: block;
        object-fit: cover;
        border-radius: 50%;
    }
}


</style>