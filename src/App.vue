<script>
  import AppHeader from "./components/AppHeader.vue";
  import AppMain from "./components/AppMain.vue";
  import AppFooter from "./components/AppFooter.vue";
  import VerticalBar from "./components/VerticalBar.vue";

  export default{
    name:"App",

    components:{
      AppHeader,
      AppMain,
      AppFooter,
      VerticalBar,
    }
  }
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
  <VerticalBar />

</template>

<style lang="scss">
@import "./styles/general.scss"
  
</style>
