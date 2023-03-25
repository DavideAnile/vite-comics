<script>
  import AppHeader from "./components/AppHeader.vue";
  import AppContent from"./components/AppContent.vue";
  import AppReferencies from"./components/AppReferencies.vue";

  export default {
    data(){
      return{

      }
    },

    components : {
      AppHeader,
      AppContent,
      AppReferencies
    }
  }

</script>

<template>
  <AppHeader></AppHeader>
  <AppContent></AppContent>
  <AppReferencies></AppReferencies>
</template>

<style>



</style>