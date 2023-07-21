<script setup>
import axios from 'axios';

function getApi() {
 

return axios.get('https://api.publicapis.org/entries')
    

}

</script>

<template>
  <div>
    <button @click="getApi">Fetch Data</button>
  </div>
</template>