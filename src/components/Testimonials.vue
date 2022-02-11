<template>
   <h1> <span style="color: #f01212;">TESTIMONIALS</span></h1>
  <div class="contai ">
   
     <div v-for="testimonial in testimonials" :key="testimonial" class="testimonial">
      <div >
        <img class="test_img" :src="testimonial.img" />
      </div>
      <div class="nam">
       <h1 class="name">{{ testimonial.title }}</h1>
      </div>
      <div class="rela">
        <h2 class="relation">{{ testimonial.relation}}</h2>
      </div>
     <div class="quo">
        <h4 class="quote" style="color:grey;">{{testimonial.quote}}</h4>
     </div>
     <div class="ema">
        <h6 class="email">{{ testimonial.email }}</h6>
     </div>
     

      
     </div>

  </div>

</template>

<script>
export default {
  data(){
    return {
      testimonials:[]
    }
  },
 
        mounted(){
            fetch('  https://myport-backend.herokuapp.com/testimonials')
            .then(res => res.json())
            .then(data => this.testimonials = data)
            .catch(err => console.log(err.message))
        }
}  


            
      
        
</script>

<style>
.contai{
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  padding-top:25px;
  overflow-y: hidden;
  padding-bottom:25px;
}
.testimonial{
  height: 600px;
  width: 380px;
  border: 1px solid lightgray;
  border-radius:9px;
  margin: 25px;
  background-color:white;
  /* padding:250px; */
  overflow-x: hidden;
  
  /* box-shadow:  1px 1px 1px 1px black; */
}

.test_img{
  display: flex;
  width: 395px;
  height: 330px;
  object-fit:cover;
    border-radius:9px 9px 0 0;
}

.name{
  font-size: 20px;
  text-align: center;
  padding-top:25px;
  font-weight: bold;
  padding:10px;
}
.relation{
  font-size:20px ;
  margin-top:5px;
   font-weight: bold;
   padding:10px;
}

.quote{
  font-size: 17px;
  text-align: center;
  padding-top:25px;
  font-weight: 30px;
  padding:10px;
  
}


.testimonial:hover{
  /* -ms-transform: scale(1.5);
  -webkit-transform: scale(1.5);  */
  transform: scale(1.1); 
  transition: 0.5s;
  
}


.email{
  padding-top:25px;
  color: #f01212;
  padding:10px;
  font-weight: bold;
}



@media only screen and (max-width: 904px){
  .testimonial{
  height: 600px;
  width: 340px;
  border: 1px solid lightgray;
  border-radius:9px;
  margin: 25px;
  background-color:white;
  /* padding:250px; */
  overflow-x: hidden;
  overflow-y: hidden;
  /* box-shadow:  1px 1px 1px 1px black; */
}

.test_img{
  display: flex;
  width: 340px;
  height: 330px;
  object-fit:cover;
    border-radius:9px 9px 0 0;
}
}
  
</style>