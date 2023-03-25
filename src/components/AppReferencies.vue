<script>
 export default{
    data(){
        return{
            referencies :[
                {
                    title : 'DC COMICS',
                    links : [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News'
                    ]
                },
                {
                    title : 'DC',
                    links : [
                        'Terms Of Use',
                        'Privacy policy (new)',
                        'Ad Choices',
                        'Advertising',
                        'Jobs',
                        'Subscription',
                        'Talent Workshops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help',
                        'Contact Us'
                    ]
                },
                {
                    title : 'SITES',
                    links : [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa'
                    ]
                },
                {
                    title : 'SHOP',
                    links : [
                        'Shop DC',
                        'Shop DC Collectibles'
                    ]
                }
            ]
        }
    }
 }
</script>

<template>
    <div class="referencies">
        <div class="my-container">
            <div class="list-container">
                <div v-for="(elemento, indice) in referencies" class="link-container">
                    <ul>
                        <li class="links-title">{{ referencies[indice].title }}</li>
                        <li v-for="link in referencies[indice].links" class="links">{{ link }}</li>
                    </ul>
                </div>
            </div>
            <div class="big-logo-container">
                <img src="/img/dc-logo-bg.png" alt="">
            </div>
        </div>

    </div>

</template>

<style lang="scss" scoped>

.referencies{
    
    width: 100%;
    height: 450px;
    background-image: url("/img/footer-bg.jpg");
    background-size: cover;

    .my-container{
        display: flex;
        justify-content: space-between;
        align-items: center;
        overflow: hidden;
       
        .list-container{
            position: relative;
            display: flex;
            justify-content: space-between;
            flex-flow: row wrap;
            gap: 40px;
           

            .link-container{
             width: 100% / 3;
             
             
                .links{
                    opacity: .5;
                }

                .links:hover{
                    cursor: pointer;
                    opacity: 1;
                }
                
                .links-title{
                    font-size: 2em;
                    font-weight: bold;
                    margin-bottom: 10px;
                 
 
                }

                
            
            }
            .link-container:last-child{
                position: absolute;
                bottom: -20px;
            }
            
        }
            
    }

}


    


</style>