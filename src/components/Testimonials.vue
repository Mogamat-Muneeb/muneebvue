<template>
   <h1> <span style="color: #f01212;">TESTIMONIALS</span></h1>
  <div class="contai ">
   
     <div v-for="testimonial in testimonials" :key="testimonial.id" class="testimonial">
      <div >
        <img class="test_img" :src="`${testimonial.img}`" />
      </div>
      <div class="nam">
       <h1 class="name">{{ testimonial.name }}</h1>
      </div>
      <div class="rela">
        <h2 class="relation">{{ testimonial.relation}}</h2>
      </div>
     <div class="quo">
        <h4 class="quote">{{testimonial.quote}}</h4>
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
                testimonials:[ {"name":" Mogamat Breda","id":1,"img":"https://i.postimg.cc/FRkTVGGL/Breda-Y1-6-11zon.jpg","email":"mugammadbreda1999@gmail.com","quote":"This man is hardworking as well as efficient with his time. Great guy to work with.","relation":"Colleague"
        },

        {"name":" Yaseen Davids","id":2,"img":"https://i.postimg.cc/k5Bs7w0p/Yaseen3-9-11zon.jpg","email":"yaaseendav@gmail.com","quote":"Muneeb is an amazing designer and is always willing to help the next person.","relation":"Colleague"
        },
        
        {"name":" Ndomizanele Moni","id":3,"img":"https://i.postimg.cc/TwbcD1Yj/Zanele3-10-11zon.jpg","email":"zanelemoni4@gmail.com","quote":"Muneeb is a good person,he is always willing to help .He is always focused on the task at hand and is not easily distracted, HE LOVES HIS WORK. ","relation":"Colleague"
        },
        
        {"name":"  Na-aim Fredericks","id":4,"img":"https://i.postimg.cc/8zkTLjVH/Na-aim3-7-11zon.jpg","email":"fredericksnaam13@gmail.com","quote":"Muneeb is a very accountable guy when it comes to being a team player he is always flexible in his work he is ethical and loyal.","relation":"Colleague"
        },
        
        {"name":" Simamkele January","id":5,"img":"https://i.postimg.cc/dv7gPntj/Simamkele2-8-11zon.jpg","email":"simamkelejanjuary@gamil.com","quote":"Besides bieng an outatanding classmate, Muneeb is a free spirited young man who is always ready to help out where he is needed.","relation":"Colleague"
        },

        {"name":"  Alex Sexwale","id":6,"img":"https://i.postimg.cc/vB4NSG8D/alex-5-11zon.jpg","email":"alexsexwale@gmail.com","quote":"Muneeeb is vigilant with his work. He continues to find ways to provide quality work and keep improving on his general knowledge.","relation":"Lecturer"
        }]
            }
        },
        // mounted(){
        //     fetch('  http://localhost:3000/testimonials')
        //     .then(res => res.json())
        //     .then(data => this.testimonials = data)
        //     .catch(err => console.log(err.message))
        // }
}  


            
      
        
</script>

<style>
.contai{
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  padding-top:25px;
}
.testimonial{
  height: 600px;
  width: 400px;
  border: 1px solid orange;
  border-radius:9px;
  margin: 25px;
  /* padding:250px; */
  
  /* box-shadow:  1px 1px 1px 1px black; */
}

.test_img{
  display: flex;
  width: 399px;
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
  
</style>