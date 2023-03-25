<script>
 export default{
    data(){
        return{
            links : [
                {
                    img : '/img/buy-comics-digital-comics.png',
                    title : 'DIGITAL COMICS'
                },
                {
                    img : '/img/buy-comics-merchandise.png',
                    title : 'DC MERCHANDISE'
                },
                {
                    img : '/img/buy-comics-subscriptions.png',
                    title : 'SUBSCRIPTION'
                },
                {
                    img : '/img/buy-comics-shop-locator.png',
                    title : 'COMIC SHOP LOCATOR'
                },
                {
                    img : '/img/buy-dc-power-visa.svg',
                    title : 'DC POWER VISA'
                }
            ]
        }
    }
 }
</script>

<template>
    <div class="main-container-section">
        <div class="my-container">
            <div v-for="elemento in links" class="link-container">
                <div class="img-container">
                    <img :src="elemento.img" alt="">
                </div>
                <div>{{ elemento.title }}</div>
                
            </div>
        </div>
    </div>
</template>

<style lang=scss scoped>

.main-container-section{
    background-color: #0282f9;
    height: 150px;


    .my-container{
        display: flex;
        justify-content: space-between;
        padding: 0 50px;
        
        

        .link-container{
            display: flex;
            align-items: center;
            gap: 10px;
            font-weight: bold;
            cursor: pointer;
            
            .img-container img{
                height: 50px;
                
            }

        }
           
        .link-container:last-child img{
            height: 30px;
        }
            
        


}
}

            
        
                
                




</style>