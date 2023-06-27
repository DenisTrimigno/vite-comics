<script>

export default{
name: "AppJumbotroon",
    data() {
        return{
    jumboList : [
     {
        nameList: "DC COMICS", 
        liss: ["Characters", "Comics","Movies","TV","Games","Videos","News"]
     },

     {
        nameList: "SHOP", 
        liss: ["Shop DC", "Shop DC Collectibles"]
     },

     {
        nameList: "DC", 
        liss: ["Term of Use", "Privacy policy(New)","Ad choices","Advertising","Jobs","Subscritions","Talent workshops","CPSC Certificates","Ratings","Shop Help","Contact Us"]
     },

     {
        nameList: "SITES", 
        liss: ["DC", "MAD Magazine","DC Kids","DC Universe","DC Power Visa"]
     }



    ]
    }
  }
}


</script>

<template>
    <section>
        <div class="container">
            
        <div class="lists">
            <ul v-for="(itm,index) in jumboList">
                <h4>{{itm.nameList}}</h4>
              <li v-for="(element) in jumboList[index].liss"><a href="">{{element}}</a></li>
            </ul>
        </div>

             <img class="logo-j" src="../assets/img/dc-logo-bg.png" alt="">
        </div>
       
    </section>
</template>

<style lang="scss" scoped>

   section{
    width: 100%;
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    height: 120vh;

     .logo-j {
    margin-left: 90vh;
    width: 140vh;
   }
  
.container{
   .lists{
    max-height: 300px;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    justify-content: flex-start;

    h4{ color: white;
        margin-bottom: 10px;
            }
            ul{
                margin-right: 30px;
                margin-bottom: 20px;
                list-style: none;

                li{
                    a{
                    
                    text-decoration: none;
                    font-size: small;
                    color: rgb(170, 170, 170);
                    }
                }
        
        
    }


   
}

   

    }
    

    }
</style>