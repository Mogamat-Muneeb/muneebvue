<template>
  <section id="home"><Home/></section>
  <section id="about"><About/></section>
  <section id="resume"><Resume/></section>
  <section id="skills"><Skills/></section>
  <section id="projects"><Projects/></section>
  <section id="testimonials"><Testimonials/></section>
  <section id="contact"><Contact/></section>
 

  
</template>

<script>
import Contact from './Contact.vue'
import Home from './Home.vue'
import Projects from './Projects.vue'
import Skills from './Skills.vue'
import Testimonials from './Testimonials.vue'
import About from './About.vue'
import Resume from './Resume.vue'

export default {
  components: {
    Contact,Home,Projects,Skills,Testimonials,About,Resume
  }
}
</script>

<style>
section{
    overflow-x: hidden;
    
}

.text:hover{
  color: #f01212;
}
.nav-item a{
  color: white !important;
}
.offcanvas-body{
  background-color:	rgb(0,0,0);
}
 
.offcanvas-end{
  width:250px;
}

.offcanvas-header{
  background-color: 	rgb(0,0,0);
  
}
  
.navbar-toggler:focus{
  box-shadow: none;
}

.navbar{
  opacity: 0.8;
}

.navbar>.container-fluid{
  justify-content: flex-end;
  background-color:none ;
}

.navbar-light .navbar-toggler{
  border: none;
}
.navbar-toggler-icon {
  opacity:1;
}

.bg-dark {
 --bs-bg-opacity: 0.0;
}
/* @media only screen and (max-width: 600px){
  section {
    display: flex;
    justify-content:center;
    height: 100vh;
  }
} */


</style>