<template>
  <div class="Qrs">
    <img class= "QR_codes" src="../assets/AME_QR.png" alt="AME code">
    <img class= "QR_codes crypto" src="../assets/Solana_QR.png" alt="solana code">
    <img class= "QR_codes crypto" src="../assets/Tezos_QR.png" alt="tezos code">
    <img class= "QR_codes crypto" src="../assets/Algorand_QR.png" alt="algorand code">
   </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>


<style scoped> 
.Qrs{
  display: flex;
  justify-content: space-between;
 }

 .QR_codes{
   margin-top: 10%;
   height:100px;
   width:100px;
 }


</style>
