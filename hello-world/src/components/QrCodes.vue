<template>
  <div class="Qr_div"> 
    <span><img class= "QR_codes" src="../assets/AME_QR.png" alt="AME code"> <CryptoPrices /></span>
    <span><img class= "QR_codes" src="../assets/Tezos_QR.png" alt="tezos code"> <TezPrice /></span>
    <span><img class= "QR_codes" src="../assets/Solana_QR.png" alt="solana code"> <SolPrice /> </span>
    <span><img class= "QR_codes" src="../assets/Algorand_QR.png" alt="algorand code"><AlPrice /> </span>
   </div>

    
</template>

<script>
import CryptoPrices from './Prices.vue'
import AlPrice from './AlgorandPrice.vue'
import SolPrice from './SolanaPrice.vue'
import TezPrice from './TezosPrice.vue'

export default  {
  name: 'QrCodes',
  components: {
    CryptoPrices,
    AlPrice,
    SolPrice,
    TezPrice,
  }
}



</script>


<style scoped> 
.Qr_div{
  display: flex;
  margin-top:15px;
  justify-content: space-around;
  border: 3px solid rgb(31, 146, 46);
  border-radius: 15px;
 }

 .QR_codes{
   margin-top: 10%;
   height:100px;
   width:100px;
 }

  img{
  border: 1px solid;
  padding: 10px;
  box-shadow: 5px 10px 0px ;
  background-color:rgb(31, 146, 46)
  }


</style>
