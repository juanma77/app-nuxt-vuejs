<template>
    <div>
        <h1 class="statement">Progress Report</h1>
        <p class="bodytext"></p>

         <p>{{ statusUpdate }}</p>
         <p>{{ statusDate }}</p>  

         <p>This is our current progress:</p>
         <ProgressBar></ProgressBar>

         <br>
         <p>Who is working right now in this?</p>

         <p>Developer: {{ barInfo.owner }}</p>
         <p>Age: {{ barInfo.age }}</p>
         <p>Location: {{ barInfo.location }}</p>
  
        <nuxt-link to="/" class="callToAction">Go Back</nuxt-link>
    </div>
</template>

<script>
import ProgressBar from '../components/ProgressBar';
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
    },
    components: {
        ProgressBar
    },
    data(){
        return {
            barInfo: {
                owner: 'John',
                age: 43,
                location: 'Virginia'  
            }
        }
    }
}
</script>

<style>

</style>