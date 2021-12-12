<template>
  <QrCodes />
  
</template>

<script>
import QrCodes from './components/QrCodes.vue'

// axios.get("https://api.coingecko.com/api/v3/simple/price?ids=tezos%2Calgorand%2Csolana&vs_currencies=usd")
// .then(res => {
//         this.res = res,
//         this.data[0] = "Tezos current price:" + res.data.tezos.usd 
//         this.data[1] = "Algorand current price:" + res.data.algorand.usd
//         this.data[2] = "Solana current price:" + res.data.solana.usd 
//         })

// const getPrices = async() => {
//   await fetch("https://api.coingecko.com/api/v3/simple/price?ids=tezos%2Calgorand%2Csolana&vs_currencies=usd")
//   .then(res => res.json())
//   .then(data => {
//     console.log(data)
//   })
// }
export default {
  name: 'App',
  components: {
    QrCodes
  }
}
</script>


