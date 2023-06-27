<script>

export default {
        name: "AppMenu",
        data(){
            return{
                links: [
                    {
                      srcIm : "../assets/img/buy-comics-digital-comics.png",
                      description: "DiGITAL COMICS"

                    },

                    {
                      srcIm : "../assets/img/buy-comics-merchandise.png",
                      description: "DC MERCHANDISE"

                    },

                    {
                      srcIm : "../assets/img/buy-comics-shop-locator.png",
                      description: "COMIC SHOP LOCATOR"

                    },

                    {
                      srcIm : "../assets/img/buy-dc-power-visa.svg",
                      description: "DC POWER VISA"

                    },

                    {
                      srcIm : "../assets/img/buy-comics-subscriptions.png",
                      description: "SUBSCRIPTOR"

                    },


                ]
            }
        }, 
        methods : {

            getImagePath: function(imgPath){

                return new URL(imgPath, import.meta.url).href

            }

        }
    }

</script>

<template>

    <section>
        <div class="container">

            <div class="card" v-for="(item) in links">

                <img :src="getImagePath(item.srcIm)" alt="">
                <a href="">{{item.description}}</a>
                
                
            </div>

        </div>
    </section>
</template>

<style lang="scss" scoped>

section{
    height: 25vh;
    background-color:  #0282F9;

    .card{
        display: flex;
        justify-content: flex-start;
        align-items: center;
        margin-right: 15px;
        width: calc(100% / 5 - 15px);
        font-size: small;

        a{
            text-decoration: none;
            color: white;
        }

        img{
            margin-right: 10px;
            max-height: 80px;
            width: 80px;
        }

    }
}



</style>