<script>

export default{
    name:"HeaderSearchbar",
}

</script>

<template>
    <div>
        <input type="text" placeholder="Search...">
        <button>
            <i class="fa-solid fa-magnifying-glass"></i>
        </button>
    </div>
</template>

<style lang="scss" scoped>
   
    input{
        outline: none;
        border: 0 solid white;
        border-radius: 10px 0 0 10px;
        padding: 1rem;
        width: 120px;
    }

    button{
        padding: 1rem;
        background-color: white;
        border: 0;
        border-radius: 0 10px 10px 0;
    }


    

</style>