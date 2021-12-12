<template>
  <div class="Alprices">
 <span id= "tezosPrice"> </span>
  </div>
</template>

<script>
import TezPrice from './TezosPrice.vue'
import axios from "axios"


export default {
  name: 'TezPrice',
  component : {
    TezPrice
  }
}

axios.get("https://api.coingecko.com/api/v3/simple/price?ids=tezos%2Calgorand%2Csolana&vs_currencies=usd")
  .then(response => {
    console.log(response.data) 
    document.getElementById('tezosPrice').textContent = "$" + response.data.tezos.usd 
    })
    .catch(error => {
      console.log("error" + error.response)

     
  })


</script>