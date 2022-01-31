<template>
  <h1> <span style="color:#f01212;">PROJECTS</span> </h1>
  <div class="holder">
       <div v-for="project in projects" :key="project.id" class="project">
      <div class="proj_box">
            <!-- <h2>{{ project.title }}</h2> -->
           <div class="bucket">
   <img class="proj_img" :src="`${project.img}`" alt="">
  <div class="overlay">
    <div class="text1 fw-bolder">{{ project.title }}</div>
    <div class="econ">
        <div class="row">
            <div class="col">
                <a :href="`${project.links.github}`"><i class="   fab fa-github"></i></a> 
            </div>
            <div class="col">
                 <a :href="`${project.links.netlify}`"><i class=" far fa-eye"></i></a>           
             </div>
            </div>
       
    </div>
   
</div>

         

  
      </div>
      </div>
      
    
  </div>
  </div>
 
</template>

<script>
export default {
        data(){
            return {
                projects:[ {"title":"E-Commerce Website","id":1,"img":"https://i.postimg.cc/8zSHpkLD/ecom1-3-11zon.png","links":{
            "github":"https://github.com/Mogamat-Muneeb/online-store",
            "netlify":"https://dinghystore.netlify.app"
        }},
        {"title":"JS Calculator","id":2,"img":"https://i.postimg.cc/8kYM5kQ9/calculator.png","links":{
            "github":"https://github.com/Mogamat-Muneeb/calculator_2",
            "netlify":"https://jscalculator2.netlify.app"
        }},
        {"title":"Box-Model","id":3,"img":"https://i.postimg.cc/PJ7WnTTG/boxmodel-2-11zon.png","links":{
            "github":"https://github.com/Mogamat-Muneeb/cards-boxmodel",
            "netlify":"https://cards-boxmodel.netlify.app"
        }},
        {"title":"Reaction-Timer","id":4,"img":"https://i.postimg.cc/JhDc345h/Screenshot-11.png","links":{
            "github":"https://github.com/Mogamat-Muneeb/reaction-time-vue-",
            "netlify":"https://muneebs-reacting-timer.netlify.app/"
        }},
        {"title":"Davids Driving School-Brochure Site","id":4,"img":"https://i.postimg.cc/J01kF1ZZ/Screenshot-10.png","links":{
            "github":"https://github.com/Mogamat-Muneeb/davids_drivingschool",
            "netlify":"https://davids-drivng-school.netlify.app"
        }}
        ]
            }
        },
        // mounted(){
        //     fetch('http://localhost:3000/projects')
        //     .then(res => res.json())
        //     .then(data => this.projects = data)
        //     .catch(err => console.log(err.message))
        // }
}
</script>

<style scoped>

.holder {
    display:flex;
    justify-content: center;
    flex-wrap: wrap;
    
    /* height:70vh; */
}
.project{
    display: flex;
    justify-content:center;
    flex-wrap: wrap;
    
}

.bucket {
     display:flex;
    justify-content: center;
    flex-wrap: wrap;
    width: 400px;
    height: 250px;
  position: relative;
  margin: 10px;
 
}

.proj_img {
  display: block;
  width: 399px;
  height: auto;
  object-fit: cover;
   border: 6px solid black;
   border-radius:2px;
  
}

.overlay {
   
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0;
  transition: .5s ease;
  background: rgba(0, 0, 0, 0.5);
}

.bucket:hover .overlay {
  opacity: 1;
}

.text1 {
  color: rgba(255, 255, 255, 1);
  font-size: 20px;
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
}


.fab{
    font-size:30px;
    display: column;
    color: white;
}
.far{
    font-size:30px;
    display: column;
    color: white;
}

.econ{
    display:flex;
    justify-content: space-evenly;
  padding-top: 130px;
}
</style>