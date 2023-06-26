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
        <img src="" alt="MaxCoach logo">
    </div>
    <nav class="header-right">
        <div class="element-nav">
            <h3>home</h3>
            <i class="fa-solid fa-angle-down"></i>
        </div>
        <div class="element-nav">
            <h3>home</h3>
            <i class="fa-solid fa-angle-down"></i>
        </div>
        <div class="element-nav">
            <h3>home</h3>
            <i class="fa-solid fa-angle-down"></i>
        </div>
        <div class="element-nav">
            <h3>home</h3>
            <i class="fa-solid fa-angle-down"></i>
        </div>
        <div class="element-nav">
            <h3>home</h3>
            <i class="fa-solid fa-angle-down"></i>
        </div>
        <div class="element-nav">
            <h3>home</h3>
            <i class="fa-solid fa-angle-down"></i>
        </div>
        <div class="element-nav">
            <span>carrello</span>
        </div>
        <div class="element-nav">
            <span>user</span>
        </div>
        <HeaderSearchbar />
    </nav>
</header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/mixins.scss" as *;

header{
    @include flex(row,space-between,center);
    padding: 0 3.5rem
}

nav.header-right{
    @include flex(row,center,center);

    .element-nav{
        padding: 1rem;
    }

    

    h3{
        display: inline;
    }
    
    
}

</style>