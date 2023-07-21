<script setup>
import HelloWorld from './components/HelloWorld.vue'
// import test from './components/test.vue'
import countries from './data/countries'

const link = {

  imageUrl: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSg-3382ZgdUhzsOz0VYE8KVNtX_HTwTxRSps08Nli1&s",
  alt: "image",
  linkUrl: "https://ostad-assignment-module3.netlify.app/",
  
} 

</script>

<template>
  <div>
    <!-- <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a> -->

  <!-- <a :href="link.linkUrl"><img :src="link.imageUrl" :alt="link.alt" style="width:500px"></a>
  <hr>
   -->
  
   <div v-for="country in countries" v-show="'B'==country.country[0]">{{ country.country }}<hr></div>



  </div>
 
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
