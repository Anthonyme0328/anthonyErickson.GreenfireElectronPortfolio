<template>
  <div class="Solprices">Solana
 <span id= "solanaPrice"> </span>
  </div>
</template>

<script>
import SolPrice from './SolanaPrice.vue'
import axios from "axios"


export default {
  name: 'SolPrice',
  component : {
    SolPrice
  }
}

axios.get("https://api.coingecko.com/api/v3/simple/price?ids=tezos%2Calgorand%2Csolana&vs_currencies=usd")
  .then(response => {
    console.log(response.data) 
    document.getElementById('solanaPrice').textContent = "$" + response.data.solana.usd 
    })
    .catch(error => {
      console.log("error" + error.response)

     
  })


</script>

<style>
 .Solprices{
   margin-top: 5%;
   font-size: 30px;
 }
</style>
