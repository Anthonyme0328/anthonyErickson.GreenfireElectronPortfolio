<template>
<div>
  <header> Crypto Prices and Twitter </header>
  <div><QrCodes /> </div>

  <div><Tweets /> </div>
  
  <div> <Links /> </div>
</div>
</template>



<script>
import QrCodes from './components/QrCodes.vue'
import Links from './components/Links.vue'
import Tweets from './components/Tweets.vue'

export default {
  name: 'App',
  components: {
    QrCodes,
    Links,
    Tweets
  }
}
</script>

<style>
*{
  font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif
}

header{
  font-size: 80px;
  text-align: center;
  border: 3px solid rgb(31, 146, 46);
  border-radius: 15px;
}
body{
  background-color: #ADEFD1FF;
}

</style>


