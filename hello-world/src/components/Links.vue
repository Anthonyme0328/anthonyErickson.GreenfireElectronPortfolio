<template>
  <div class= "links">
      <a href="https://github.com/Anthonyme0328">GitHub | </a>
      <a href="https://www.linkedin.com/in/anthony-erickson-42621b1b9/">LinkedIn | </a>
      <a href="mailto:anthonymh14@hotmail.com">Email | </a>
      <a href="https://docs.google.com/document/d/1eGGUCS_5ncUKAyP-d-pD08Bs-b83V8wbL8R3ndSglHU/edit?usp=sharing">Resume | </a>
      <a href="https://anthonyme0328.github.io/Bootstrap-Portfolio/">Website</a>
  </div>

</template>


<script>
import Links from './Links.vue'

export default ({
  name: Links,
   component: {
    Links
  },
})
</script>

<style>
.links{
    position: absolute;
    bottom: 0;
    margin-left: 60vh;
    margin-right: 60vh;
    font-size: 45px

}

.links:hover{
  
}
</style>
