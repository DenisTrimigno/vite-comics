<script>
export default {
  data(){
    return{
         icons : 
         [


         ]
    };
  },
}
</script>

<template lang="">
  <main>
    <div class="black">
      <div class="container">
        <h1>Content goes here </h1>
      </div>
    </div>
    <div class="blue">
      <div class="container">
        <ul>
          <li v-for="(link, index) in links" :key="index" :class="link.active ? 'active' : ''">
                <a :href="link.href" >
                    {{ link.label }}
                </a>

          </li>
        </ul>
      </div>
    </div>
  
  </main>
 
</template>

<style lang="scss" scoped>
    .black{
      background-color: rgb(0, 0, 0);
    }

    h1{
      padding: 40px;
      color: white;
    }

    .blue {
      background-color: blue;
    }
  
</style>