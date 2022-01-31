<template>
  <h1> <span style="color:#f01212;"> SKILLS</span> </h1>
  <div class="contain d-flex justify-content-center">
    <div class="row">

      <div class="col-sm-4">
        <div class="lang">
     <span class=" icon icon1"> <i class="fab fa-html5"></i></span>
      
      </div>
      <h4 class="h4">HTML</h4>
       <div class="lang">
     <span class="icon icon2"> <i class="fab fa-css3-alt"></i></span>
  
      </div>
         <h4 class="h4">CSS</h4> 
     
      </div>
      
      <div class="col-sm-4">
          <div class="lang">
     <span class=" icon icon3"> <i class="fab fa-js"></i></span>
    
      </div>
       <h4 class="h4">JAVASCRIPT</h4> 
         <div class="lang">
     <span class="icon icon4"> <i class="fab fa-bootstrap"></i></span>
     
      </div>
       <h4 class="h4">BOOTSTRAP</h4>
      </div>
      
      
      <div class="col-sm-4">
       <div class="lang">
     <span class=" icon icon5"> <i class="fab fa-git-alt"></i></span>
     
      </div>
       <h4 class="h4">GIT</h4>
       <div class="lang">
     <span class="icon icon6"> <i class="fab fa-vuejs"></i></span>
     
      </div>
      <h4 class="h4">VUE.JS</h4> 
      </div>
      

    </div>
  </div>
 
 

 
</template>

<script>
export default {

}
</script>

<style>

.container {
  display:flex;
  justify-content:space-around;
  /* height:70vh; */
}
.h4{
  font-size: bold;
  text-align:center !important;
  margin-right: 35px;
  padding-top: -100px;
}
.lang {
  display:flex;
  justify-content:space-between;
  padding: 70px;
}
.icon {
  font-size: 150px;
  margin: 0 auto;
  display:flex;
  justify-content:space-between;
}

.icon1:hover{
  color:  #F06529;
  transition:0.5s;
}
.icon2:hover{
  color: #e31b5f;
  transition:0.5s;
}

.icon3:hover{
  color: #F0DB4F;
  transition:0.5s;
}
.icon4:hover{
  color: #602C50;
  transition:0.5s;
}
.icon5:hover{
  color: #F1502F;
  transition:0.5s;
}
.icon6:hover{
  color: #41B883;
  transition:0.5s;
}
@media only screen and (max-width: 600px){
 .contain{
   display: flex;
   justify-content: center;
   margin-left: 50%;
   margin-right:50% ;
 }
 .lang{
   padding:30px;
 }
/*  
.icon1{
  color:  #F06529;
  
}
.icon2{
  color: #e31b5f;
  
}

.icon3{
  color: #F0DB4F;
  
}
.icon4{
  color: #602C50;
  
}
.icon5{
  color: #F1502F;
  
}
.icon6{
  color: #41B883;
  
} */
}
</style>