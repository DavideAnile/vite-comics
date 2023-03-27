<script>
    export default {
        
        data(){
            return{

            }
        },

        props : {
            title : String,
            img : String,
        }
    }
</script>


<template>
<div class="card-container">

    <div class="thumb-container">
        <img :src= img alt="">
    </div>
    <div class="cardTitle"> {{ title }} </div>

</div>

</template>

<style lang="scss" scoped>

.card-container{
    width: calc(100% / 6 - (40px / 6 * 5));
    
    

    
    
    
    .thumb-container{
        width: 100%;
        height: 200px;
        cursor: pointer;
        

        img{
           
           width: 100%;
           height: 100%; 
           object-fit: cover;
           object-position: top;
           
        }
    }

    .cardTitle{
        padding: 15px 0;
        text-align: center;
        text-transform: uppercase;
    }
}

</style>