<template>
  <h1>  <span  style="color:#f01212;"> RESUME</span></h1>
  <div class="container">
     <div class="timeline">
         <h3>Education</h3>
  <div class=" col outer">
    <div class="card">
      <div class="info">
        <h4 class="date"> 2015-2020:</h4>
        <h3 class="title">Vootrekker High School</h3>
        <p>I started and ended my high school career at Vootrekker High School in Kenilworth. I was part of the RCL leadership team from Gr.10 to Gr.12 and played First-Team rugby since Gr.10 as a Scrumhalf. I was the Deputy Head Boy in Matric and also matriculated in the year 2020.</p>
      </div>
    </div>
    <div class="card">
      <div class="info">
        <h4 class="date">  2021-Present:</h4>
        <h3 class="title">Life Choices Coding Academy</h3>
        <p>A Bootcamp program that gives you the care fundamentals of Web Development, learning coding languages such as HTML, CSS, Javascript and more coding techniques. We are aso taught interpersonal and self-development skills to take us further in life. </p>
      </div>
    </div>
  </div>
</div>

 <div class="timeline">
         <h3> Work & Experience</h3>
  <div class=" col outer">
    <div class="card">
      <div class="info">
         <h4 class="date"> 2014-2018:</h4>
        <h3 class="title">Project Maritime Youth Naval Cadet School</h3>
        <p>Every Saturday for 4 years I spent my day practising naval and survival skills.I was also an instructor and PTI officer. My leadership and discpline was improved due to harsh and intense physical training.</p>
      </div>
    </div>
    <div class="card">
      <div class="info">
         <h4 class="date"> Start of 2021:</h4>
        <h3 class="title">Kieth Sealants and Projects</h3>
        <p> I was an apprentice learning general building techniques.</p>
      </div>
    </div>
    <div class="card">
      <div class="info">
         <h4 class="date"> 2020-present:</h4>
        <h3 class="title">Volunteering</h3>
        <p> Started tutoring and helping out at Muslim school,teaching kids how to recite the quran and basic fundamentals of Islam and tutoring mathematics to grade 9 learners.</p>
      </div>
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
.container{
  display: flex;
  flex-wrap: wrap;
}

.date{
  font-size:13px;
}
:root {
  --primary-color: #fff; /* try #212121 also for dark mode */
  --background-color: #212121;
  --font: sans-serif;
}

/* * {
  margin: 0;
  padding: 0;
} */

body {
  /* background: var(--background-color);
  font-family: var(--font); */
  /* display: flex;
  justify-content: center; */
}

/* Timeline Container */
.timeline {
  background: var(--primary-color);
  margin: 20px auto;
  padding: 20px;
}

/* Outer Layer with the timeline border */
.outer {
  border-left: 2px solid #333;
}

/* Card container */
.card {
  position: relative;
  margin: 0 0 20px 20px;
  padding: 10px;
  /* background: #333; */
  color: gray;
  border-radius: 8px;
  /* max-width: 400px; */
  width: 500px;
  font-size: 15px;
}

/* Information about the timeline */
.info {
  display: flex;
  flex-direction: column;
  gap: 10px;
}

/* Title of the card */
.title {
  color: #f01212;
  position: relative;
  font-size:19px;
}

/* Timeline dot  */
.title::before {
  content: "";
  position: absolute;
  width: 10px;
  height: 10px;
  background: white;
  border-radius: 999px;
  left: -37.5px;
  border: 3px solid #f01212;
}



@media only screen and (max-width: 600px){
 .card{
   width:90%;
 }
}
</style>