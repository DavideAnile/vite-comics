<script>

import AppContentSection from "./AppContentSection.vue"


    export default{
        data(){
            return{

            }
        },

        components : {
            AppContentSection
        }
         
    }
</script>

<template>
    <div class="my-container">
        <div class="content"> --&gt; Content goes here &lt;-- </div>
    </div>
    <AppContentSection></AppContentSection>
</template>

<style lang="scss" scoped>

    .my-container{
        display: flex;
        
        justify-content: center;   
        .content{
            display: flex;
            justify-content: center;
            align-items: center;
            height: 120px;
            font-size: 2em;
            font-weight: bold;
        }

    }

</style>