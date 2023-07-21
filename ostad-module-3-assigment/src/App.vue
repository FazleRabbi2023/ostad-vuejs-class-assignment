<script setup>
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
import navigation from './components/navigation.vue'
import hero from './components/hero.vue'
import section1 from './components/section1.vue'
import section2 from './components/section2.vue'
import section3 from './components/section3.vue'
import section4 from './components/section4.vue'
import section5 from './components/section5.vue'
import section6 from './components/section6.vue'
import section7 from './components/section7.vue'
import section8 from './components/section8.vue'
import section9 from './components/section9.vue'
import section10 from './components/section10.vue'
import footersection from './components/footersection.vue'

</script>

<template>
  <!-- <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div> -->
  <!-- <HelloWorld msg="Vite + Vue" /> -->
  <navigation />
  <hero />
  <section1 />
  <section2 />
  <section3 />
  <section4 />
  <section5 />
  <section6 />
  <section7 />
  <section8 />
  <section9 />
  <section10 />
  <footersection />

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
