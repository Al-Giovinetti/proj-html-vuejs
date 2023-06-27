<script>
import HeaderSearchbar  from "./HeaderSearchbar.vue"
export default{
    name:"AppHeader",

    components:{
        HeaderSearchbar,
    }
}

</script>

<template>
<header>
    <div class="header-left">
        <img src="../assets/img/light-logo.png" alt="MaxCoach logo">
    </div>
    <nav class="header-right">
        <div class="element-nav">
            <h4>Home</h4>
            <i class="fa-solid fa-angle-down"></i>
        </div>
        <div class="element-nav">
            <h4>Pages</h4>
            <i class="fa-solid fa-angle-down"></i>
        </div>
        <div class="element-nav">
            <h4>Courses</h4>
            <i class="fa-solid fa-angle-down"></i>
        </div>
        <div class="element-nav">
            <h4>Features</h4>
            <i class="fa-solid fa-angle-down"></i>
        </div>
        <div class="element-nav">
            <h4>Blog</h4>
            <i class="fa-solid fa-angle-down"></i>
        </div>
        <div class="element-nav">
            <h4>Shop</h4>
            <i class="fa-solid fa-angle-down"></i>
            <i class="fa-solid fa-cart-shopping"></i>
        </div>
        <div class="element-nav">
            <i class="fa-regular fa-circle-user"></i>
        </div>
        <HeaderSearchbar />
    </nav>
</header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/mixins.scss" as *;
@use "../styles/partials/variables.scss" as*;

header{
    @include flex(row,space-between,center);
    padding: 1.7rem 5rem;
    background-color: $bg-primary;
    color: white;
}

.header-left img{
    width: 150px;
}

nav.header-right{
    @include flex(row,center,center);
    .element-nav{
        padding: 0 0.9rem;
    }
    h4{
        display: inline;
    }
}

i.fa-angle-down{
    font-size: small;
    padding: 0 0.5rem;
}

i.fa-cart-shopping,
i.fa-circle-user{
    font-size: 1.3rem;
}


</style>