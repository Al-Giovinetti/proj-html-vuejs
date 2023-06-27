<script>


export default{
    name:"TalkAbout",

    data(){
        return{
            partners:[]
        }
    }

}

</script>

<template>
    <section>
        <h2>Why People Talk About MaxCoach?</h2>
        <div class="d-flex">
            <div class="box-img">
                <img src="" alt="partner">
            </div>
            <div class="info-box">
                <p>aaaaaaaaaa</p>
                <span>aaa</span>
                <span>aaa</span>
            </div>
        </div>
        <div class="d-flex">
            <img src="" alt="" v-for="partner in partners">aaaaaaaaaaa
        </div>
    </section>

</template>

<style lang="scss" scoped>
section{
    text-align: center;
}

</style>