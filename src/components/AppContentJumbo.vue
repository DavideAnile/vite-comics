<script>
    export default {
       
        data(){
            return{

            }
        }
    }
</script>

<template>
 <div class="jumbo-container">
    <img src="/img/jumbotron.jpg" alt="">
    <div class="series">Current series</div>
 </div>
</template>

<style lang="scss" scoped>

.jumbo-container{
    position: relative;
    width: 100%;
    height: 400px;

    img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: top;
    }

    .series{
        
        position: absolute;
        bottom: -20px;
        left: 220px;
        font-size: 1.5em;
        font-weight: bold;
        background-color: #0282f9;
        padding: 2px 20px;
        text-transform: uppercase;
    }
}

</style>