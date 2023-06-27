<script>

export default{
    name:"HelpLearn",
}

</script>

<template>
    <section>
        <p>aaaaaaa</p>
        <h2>Glad to Help You Learn</h2>
        <div class="container">
            <div>
                <i>bandiera</i>
                <span>aaaa</span>
                <p>aaaa</p>
            </div>
            <div>
                <i>bandiera</i>
                <span>aaaa</span>
                <p>aaaa</p>
            </div>
            <div>
                <i>bandiera</i>
                <span>aaaa</span>
                <p>aaaa</p>
            </div>
            <div>
                <i>bandiera</i>
                <span>aaaa</span>
                <p>aaaa</p>
            </div>
        </div>
        <img src="aaaaaaaa" alt="">
        <p>aaaaa</p>
        <p>aaaaaaaaaaaaaaa</p>
        <button>aaaaa</button>
    </section>

</template>

<style lang="scss" scoped>
@use "../../styles/partials/mixins.scss" as * ;

div.container{
    @include flex(row,space-around,start)
}
</style>