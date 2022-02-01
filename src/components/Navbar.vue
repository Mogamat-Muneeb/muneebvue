<template>
     <nav class="navbar navbar-light bg-dark fixed-top">
      <div class="container-fluid">
        <!-- <a class="navbar-brand " href="home.html">Davids Driving School</a> -->
        <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar" aria-controls="offcanvasNavbar">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="offcanvas offcanvas-end" tabindex="-1" id="offcanvasNavbar" aria-labelledby="offcanvasNavbarLabel">
          <div class="offcanvas-header">
            <h5 class="offcanvas-title" id="offcanvasNavbarLabel"></h5>
            <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
          </div>
          <div class="offcanvas-body" id="off-body">
            <ul class="navbar-nav justify-content-end ">
              <li class="nav-item d-flex justify-content-start">
                <a class=" nav-link active" aria-current="page" href="#home"><span class="text" @click=" collapse"> HOME</span> </a>
              </li>           
              <li class="nav-item  d-flex justify-content-start">
                <a class="nav-link" href="#about"  @click=" collapse"> <span class="text">ABOUT</span></a>
              </li>
              <li class="nav-item  d-flex justify-content-start">
                <a class="nav-link" href="#resume"  @click=" collapse"> <span class="text">RESUME</span></a>
              </li>
              <li class="nav-item  d-flex justify-content-start">
                <a class="nav-link" href="#skills"  @click=" collapse"> <span class="text">SKILLS</span></a>
              </li>
              <li class="nav-item  d-flex justify-content-start">
                <a class="nav-link" href="#projects"  @click=" collapse"> <span class="text">PROJECTS</span></a>
              </li>
              <li class="nav-item  d-flex justify-content-start">
                <a class="nav-link" href="#testimonials"  @click=" collapse"> <span class="text">TESTIMONIALS</span></a>
              </li>
              <li class="nav-item  d-flex justify-content-start">
                <a class="nav-link" href="#contact"  @click=" collapse"> <span class="text">CONTACT ME</span></a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </nav> 
</template>

<script>
export default {
 methods: {
     collapse(){
    let navcollapse = document.getElementsByClassName("offcanvas")[0]

    navcollapse.classList.toggle("show")
}


 },
}


</script>

<style>


.btn-close {
  opacity: 1;
  
}

.navbar-toggler-icon {
    opacity: 1;
}
.offcanvas-backdrop{
    background: none;
}

.btn-close.text-reset {
    border: none !important;
  
    
}



@media only screen and (max-width: 600px){
 .navbar-nav{
  padding-top: 70%;
  padding-bottom: 70%;
}
}
</style>