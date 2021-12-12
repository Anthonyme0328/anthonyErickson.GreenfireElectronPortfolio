<template>
  <div class="Alprices">
 <span id= "algorandPrice"> </span>
  </div>
</template>

<script>
import AlPrice from './AlgorandPrice.vue'
import axios from "axios"


export default {
  name: 'AlPrice',
  component : {
    AlPrice
  }
}

axios.get("https://api.coingecko.com/api/v3/simple/price?ids=tezos%2Calgorand%2Csolana&vs_currencies=usd")
  .then(response => {
    console.log(response.data) 
    document.getElementById('algorandPrice').textContent = "$" + response.data.algorand.usd 
    })
    .catch(error => {
      console.log("error" + error.response)

     
  })


</script>