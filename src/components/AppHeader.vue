<script>
    export default {
        data(){
            return{
                links : [
                    'Characters',
                    'Comics',
                    'Movies',
                    'tv',
                    'Games',
                    'collectibles',
                    'videos',
                    'fans',
                    'news',
                    'shop'
                ],

                activeIndex : 0
            }
        },

        methods : {
            setIndex(linkIndex){

                this.activeIndex = linkIndex

            }
        }
    }
</script>

<template>
  <nav>
    <div class="my-container">
        <div class="img-container">
            <img src="/img/dc-logo.png" alt="">
        </div>
        <ul>
            <li v-for="(link, indice) in links" @click="setIndex(indice)" :class="activeIndex == indice ? 'active' : '' ">{{ link }}</li>
            
        </ul>
    </div>
        
        
  </nav>
</template>

<style lang="scss" scoped>

nav{
    display: flex;
    align-items: center;
    height: 100px;
    background-color: white;
    color: black;

   
    .my-container{

        display: flex;
        justify-content: space-between;
        .img-container{
            width: 100px;
            height: 100%;
            padding: 20px;
    
            img{
                height: 100%;
            }
        }
    
        ul{
            display: flex;
            height: 100%;
           li{
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 8px;
            font-weight: bold;
            border-bottom: 2px solid transparent;
            cursor: pointer;
            
            &.active{
                color: blue;
                border-bottom: 2px solid blue;
                }
                
           }    
        }

    }   
        
    }

</style>