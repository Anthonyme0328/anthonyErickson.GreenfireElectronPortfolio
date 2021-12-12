<template>
  <div class="Qr_div">
    <img class= "QR_codes" src="../assets/AME_QR.png" alt="AME code">    
    <img class= "QR_codes" src="../assets/Tezos_QR.png" alt="tezos code">
    <img class= "QR_codes" src="../assets/Solana_QR.png" alt="solana code">
    <img class= "QR_codes" src="../assets/Algorand_QR.png" alt="algorand code">
   </div>
</template>

<script>
export default {
  name: 'QrCodes',
}
</script>


<style scoped> 
.Qr_div{
  display: flex;
  justify-content: space-between;
 }

 .QR_codes{
   margin-top: 10%;
   height:100px;
   width:100px;
 }


</style>
