<script>
  import AppHeader from "./components/AppHeader.vue";
  import AppContent from"./components/AppContent.vue";
  import AppReferencies from"./components/AppReferencies.vue";
  import AppFooter from"./components/AppFooter.vue";

  export default {
    data(){
      return{

      }
    },

    components : {
      AppHeader,
      AppContent,
      AppReferencies,
      AppFooter
    }
  }

</script>

<template>
  <AppHeader></AppHeader>
  <AppContent></AppContent>
  <AppReferencies></AppReferencies>
  <AppFooter></AppFooter>
</template>

<style>



</style>