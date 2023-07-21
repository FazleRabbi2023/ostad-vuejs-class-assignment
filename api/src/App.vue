<script setup>
import countries from './data/countries'

function findB(string) {
  const regex = /[A-Z]/g;
  return string.match(regex);
}

</script>

<template>
  <div>
    <h2>Countries whose names start with 'B'</h2>
   <div v-for="country in countries" v-show="'B'==findB(country.country)[0]">{{ country.country }}<hr></div>
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
