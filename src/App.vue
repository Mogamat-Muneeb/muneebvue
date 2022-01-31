<template>
<Navbar/>
<Sections/>
<Footer/>
</template>

<script>
import Navbar from "./components/Navbar.vue"  
import Sections from "./components/Sections.vue"
import Footer from "./components/Footer.vue"

export default {
  name: 'App',
  components: {
    Navbar,Sections,Footer
  }
}
</script>

<style>
#app {
 font-family: "Source Sans Pro", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
  /* width: 200%; */
  /* background-color:#0b2542 ; */
}
body{
  overflow-x: hidden;
  /* background-color: 	#d8e7f7; */
  

}


</style>
