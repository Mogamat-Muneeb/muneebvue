<template>
<!-- <h1>Home page</h1>   -->
<div class="img-slider">
  <div class="slider-container">
    

    <div class="slide">
      <img src="../assets/desk3.jpg">
    </div>
    
    <div class="slide">
      <img src="../assets/pexels-photo-269323-min.jpg">
    </div>
    
     
    <div class="slide">
      <img src="../assets/desk2.jpg">
    </div>

   
    
  </div>
</div>
<div class="words">
  <h4 class="fw-bolder"><span style="color:#2c3e50;">HI,THIS IS....</span></h4>
  <br>
   <h1 class="fw-bolder"> <span style="color:white">Mogamat Muneeb Davids</span> </h1>
   
    <h4 class="fw-bolder"><span style="color:#2c3e50">AN ASPIRING FULL STACK DEVELOPER</span></h4>
    <br>
    
 <div class="social-menu">
        <ul>
            <li><a href="https://github.com/Mogamat-Muneeb" target="blank"><i class="fab fa-github"></i></a></li>
            <!-- <li><a href="https://www.instagram.com/muneeb_davids/" target="blank"><i class="fab fa-instagram"></i></a></li> -->
            <li><a href="https://www.linkedin.com/in/mogamat-muneeb-014769224/" target="blank"><i class="fab fa-linkedin-in"></i></a></li>
            <li><a href="https://codepen.io/your-work" target="blank"><i class="fab fa-codepen" target="blank"></i></a></li>
            <!-- <li><a href="https://app.netlify.com/teams/mogamat-muneeb/overview" target="blank"><i class="fa fa-link" target="blank"></i></a></li> -->

        </ul>
  </div>
    <!-- <div class="button">
  <div class=" btn btn-outline-dark">LEARN MORE ABOUT ME</div>
</div> -->
</div>


</template>

<script>
export default {
    
}
</script>

<style>


body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;

}

.img-slider {
    position: relative;
    width: 100vw;
    height: 100vh;
    overflow-x: hidden;
    opacity: 0.9;
}
.img-slider .slider-container {
    position: absolute;
    width: 300%;
    top: 0;
    left: 0;
    overflow: hidden;
    animation: slider 8s infinite;
}
.img-slider .slider-container .slide {
    position: relative;
    width: 33.33333333%;
    height: 100vh;
    float: left;
    overflow: hidden;
    
}
.img-slider .slider-container .slide img {
  object-fit: cover;
  display: block;
  width: 100%;
  height: 100%;
}
@keyframes slider {
    0%, 25%, 100%{left: 0}
    
    30%, 55%{left: -100%}
    
    60%, 85%{left: -100%}
}

.words{
  display:flex;
  justify-content: center;
  flex-direction: column;
  position: absolute;
  top: 0;
  height: 100vh;
  width: 100%;
}

/* icons */
/* .buttons-container{
  display: flex;
  justify-content: space-around;
} */

.social-menu ul{
    position: absolute;
    top: 50%;
    left: 50%;
    padding: 0;
    margin: 0;
    transform: translate(-50%, -50%);
    display: flex;
    padding-top:200px;
}

.social-menu ul li{
    list-style: none;
    margin: 0 15px;
}

.social-menu ul li .fab{
    font-size: 30px;
    line-height: 50px;
    transition: .3s;
    color: #000;
    
}
.social-menu ul li .fa{
    font-size: 30px;
    line-height: 50px;
    transition: .3s;
    color: #000;
    
}

.social-menu ul li .fab:hover{
    color: #fff;
}
.social-menu ul li .fa:hover{
    color: #fff;
}

.social-menu ul li a{
    position: relative;
    display: block;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background-color: #fff;
    text-align: center;
    transition: .6s;
    box-shadow: 0 5px 4px rgba(0,0,0,.5);
}

.social-menu ul li a:hover{
    transform: translate(0, -10%);
}

.social-menu ul li:nth-child(1) a:hover{
    background-color: rgba(0, 0, 0, 0.829);
}
.social-menu ul li:nth-child(2) a:hover{
    background-color: #E4405F;
}
.social-menu ul li:nth-child(3) a:hover{
    background-color: #0077b5;
}
.social-menu ul li:nth-child(4) a:hover{
    background-color: #000;
}
.social-menu ul li:nth-child(5) a:hover{
    background-color: rgb(0, 187, 255);
}

</style>