<script>
    export default{
        data(){
            return{

            }
        }
    }
</script>

<template>
    <div class="footer">
        <div class="my-container">
            <div class="left-footer"><button>SIGN-UP NOW!</button></div>
            <div class="right-footer">
                <div>FOLLOW US</div>
                <div>
                    <i class="fa-brands fa-facebook"></i>
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-youtube"></i>
                    <i class="fa-brands fa-pinterest"></i>
                    <i class="fa-solid fa-location-dot"></i>
                </div>


            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>

.footer{
    width: 100%;
    height: 100px;
    background-color: #303030;

    .my-container{
        display: flex;
        justify-content: space-between;
        align-items: center;

        .left-footer button{
            padding: 10px;
            border: 1px solid #0282f9;
            background-color: transparent;
            font-weight: bold;
            cursor: pointer;
        }

        .right-footer{
            display: flex;
            align-items: center;
            gap: 20px;
            font-size: 1.4em;
            cursor: pointer;
            
        }

        .right-footer div:first-child{
            color: #0282f9;
            font-weight: bold;
            font-size: .7em;
            
            
        }

        .right-footer div:last-child{
            display: flex;
            gap: 15px;
            font-size: 1.2em;
        }

        .right-footer div:last-child i{
            opacity: .5;
        }
            

        .right-footer div:last-child i:hover{
            opacity: 1;
            transform: scale(1.3);
        }
    }
}

</style>