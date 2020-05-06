<template>
    <div>
        <h1 class="statement">Progress Report</h1>
        <p class="bodytext"></p>

         <p>{{ statusUpdate }}</p>
         <p>{{ statusDate }}</p>  
  

        <nuxt-link to="/" class="callToAction">Go Back</nuxt-link>
    </div>
</template>

<script>
const axios = require('axios');
export default {
    // We need to use "asyncData" to make the axios call
    asyncData({ params }){
        return axios.get('http://localhost:3000/status.json').then((res) =>{
            console.log(res.data);
            return{
                statusUpdate: res.data.statusUpdate,
                statusDate: res.data.statusDate
            }
        })
    }
}
</script>

<style>

</style>