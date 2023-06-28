<script>

  export default{
    name:"VerticalBar",

  }
</script>

<template>
    <div class="vertical-bar">
        <i class="fa-solid fa-ruler-combined"></i>
        <i class="fa-regular fa-life-ring"></i>
        <i class="fa-solid fa-book"></i>
        <i class="fa-solid fa-cart-shopping"></i>
    </div>

</template>

<style lang="scss" scoped>
@use "../styles/partials/mixins.scss" as *;

div.vertical-bar{
    @include flex(column,center,center);
    background-color: white;
    border: 1px solid grey;
    position: fixed;
    right: 0;
    top: 30%;
    i{
        padding: 0.7rem 0.5rem;
    }

}

   


</style>