<template>
  <div class="prices">AME
 <span id= "AMEprice">$100 </span>
  </div>
</template>

<script>
import CryptoPrices from './Prices.vue'
import axios from "axios"


export default {
  name: 'CryptoPrices',
  component : {
    CryptoPrices
  }
}

axios.get("https://api.coingecko.com/api/v3/simple/price?ids=tezos%2Calgorand%2Csolana&vs_currencies=usd")
  .then(response => {
    console.log(response.data) 
    })
    .catch(error => {
      console.log("error" + error.response)

     
  })


</script>

<style >
   .prices{
   margin-top: 5%;
   font-size: 30px;
 }
</style>