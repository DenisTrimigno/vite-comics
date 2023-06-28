<script>
export default {
  name: "AppFooter",

  data() {
    return {
      images : 
      [
        {src: "../assets/img/footer-facebook.png"},
        {src: "../assets/img/footer-periscope.png"},
        {src: "../assets/img/footer-pinterest.png"},
        {src: "../assets/img/footer-twitter.png"},
        {src: "../assets/img/footer-youtube.png"}
    ]


    }
  },


methods: {
  getImagePath: function(imgPath) {

    return new URL (imgPath, import.meta.url).href
  }
}
}
</script>

<template lang="">
  <footer>
 <div class=" background-black">
    <div class="container">
      <div class="flex justify-between align-center">
        <button>SIGN-UP NOW</button>
        <h4>FOLLOW US</h4>
        <ul class="flex justify-between align-center">
              <li v-for="(item) in images">
                   <a href=""><img :src="getImagePath(item.src)" alt=""></a>
              </li>
        </ul>
      </div>
    </div>
  </div>
  </footer>
 
</template>

<style lang="scss">

footer {
  display: inline-block;
  width: 100%;
}

  .background-black{
    background-color: rgb(45, 45, 45);
    height: 20vh;

  }

  button {
    color: white;
    background-color: transparent;
    border-color: rgb(0, 119, 255);
    padding: 10px;
    margin-right: 100vh;
  }

  h4{
    margin-right: 50px;
    color:rgb(0, 132, 255) ;
  }

  ul li {
    margin-left: 10px;
  }
  
</style>