<template>
<div class="container">
    
<div class="row row1 d-flex justify-content-center">
    <h1 class="headin d-flex justify-content-center"><span  style="color: #f01212;">ABOUT ME</span> </h1>
  <div class="box d-flex justify-content-center  col-sm-6 ">
      <img class="photo" src="../assets/Muneeb.jpg" alt="" >
  </div>

  <div class="col-sm-6">
  <h1 class="hi">Hi Guys!</h1>
  <h6 class="d-flex justify-content-start fw-bold">Bio:</h6>
  <p>I am a person that works hard and is committed to whatever I am doing at the present moment. I try my best to be punctual at my studies or anything that needs my full attention. Furthermore, I am a person that is always willing to assist and help others when in need. I love public speaking and I am very comfortable around lots of people. I am a very open person and confident.</p>
  <h6  class=" heading fw-bold">Where my passion for coding started:</h6>
  <p>My passion for the tech/coding industry started when I wanted to start my own YouTube channel. I had to do research on how to start, what I needed and what skills were needed for me to become a successful YouTuber. I developed the passion because everything we do includes having to know the tech industry.</p>
 
  <div class="about-profile">   
<ul class="admin-profile">

<li><span class="pro-title"> D.O.B      </span> <span class="pro-detail">20/08/2001</span></li>
<li><span class="pro-title"> Country    </span> <span class="pro-detail">South Africa</span></li>
<li><span class="pro-title"> Location   </span> <span class="pro-detail">Cape Town</span></li>
<li><span class="pro-title"> e-mail     </span> <span class="pro-detail">davimuneeb785@gmail.com</span></li>
<li><span class="pro-title"> Phone      </span> <span class="pro-detail">+ (27) 76 162 1649</span></li>
<li><span class="pro-title"> Freelance  </span> <span class="pro-detail">Available</span></li>
</ul>
</div>

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
    flex-wrap: wrap;
    
}
.photo{
     display: flex;
     justify-content: center;
     height: 450px;
    width: 380px;
    object-fit:cover;
    padding-right: 10px;
     /* border: 3px solid; */
}
.hi{
    display: flex;
    justify-content: center;
    padding-top:70px;
}
.admin-profile{
    display: grid;
    justify-content: center;
    padding-left: 30px;
}
.row{
    text-align:left ;
    margin-top:9%;
    margin-bottom:15%;
}

.headin {
    display:flex;
    justify-content:center;
    margin: top 3rem;
}
.box{
    display: flex;
    /* justify-content:left; */
    /* border: 3px solid; */
    height: 350px;
    width: 350px;
    /* border-radius:50%; */
    margin-top: 190px;
}
.about-profile .pro-detail{
    text-align:auto !important;
    
}
.about-profile li{
    display: flex;
    /* justify-content:space-between; */
    width:300px;
}
.about-profile .pro-title {
    font-weight: 700;
    color: #2c3e50;
    position: relative;
    width: 120px;
    display: inline-block;
    margin-bottom: 5px;
    
}

.pro-title{
    margin-left: -183px;
}

.about-profile .pro-title:after {
    position: absolute;
    content: ':';
    color: #2c3e50;
    font-size: 14px;
    left: 100px;
   
}

ul li, ol li {
    list-style: none;
}

@media only screen and (max-width: 1000px){
  .photo {
        height: 400px;
  }

  .row{
    text-align:none;
    
}
.about-profile{
    font-size:-15px ;
}
}

@media only screen and (max-width: 600px){
   .row{
    text-align:left !important;
   }
    .pro-title{
 
     margin-left:-95px;
    text-align:left !important;
}
}



@media only screen and (max-width: 720px){
   .row{
    text-align:left !important;
   }
    .pro-title{
 
     margin-left:-120px;
    text-align:left !important;
}
}


@media only screen and (max-width: 535px){
   .row{
    text-align:left !important;
   }
    .pro-title{
 
     margin-left: -150px;
    text-align:left !important;
}
.about-profile{
    margin-right:-50%;
}
}

</style>