<script>
    import Carousel from 'svelte-carousel'
    import DocturePoly from "./DocturePoly.png"
    import Nebiro from "./nebiro.png"
    import Jananya from "./jananya.png";
    import Medmokk from './medmokk.png'
    import Project_Details from './project_details.svelte'

    import Python from './python.png'
import Svelte from './svelte.png'
import React from './react.png'
import Ionic from './ionic.png'
import { SvelteComponent } from 'svelte/internal';
    let carousel; // for calling methods of the carousel instance
 
  </script>
  
  <Carousel>
    <div class="item float">
      <Project_Details 
      title="Medmokk"
      name={Medmokk} 
      des="A user interface for oral scanning checkup and connecting with dentists "
      tech={[Python,React]}
      />
    </div>
<div class="item ">
 <Project_Details
 title="DocturePoly" 
 name={DocturePoly} 
 des=" Docturepoly is a vital monitoring device for monitoring patients"
 tech={[Svelte,Ionic]}
 />
  </div>
 
 

<div class="item float">
  <Project_Details 
  title="Nebiro"
  name={Nebiro} 
  des="Diagnostic and therapeutic device for chronic COPD/ asthama patients."
  tech={[React,Ionic]}
  />
   
</div>
<div class="item float">
  <Project_Details 
  title="Jananya"
  name={Jananya} 
  des="A desktop based platform for monitoring intrapartum patients"
  tech={[Python,React]}
  />
</div>


</Carousel>
  <style>
   img{
      margin:20px;
      width:30vw;
      height:25vh;
      border-radius: 10px;
      border:dashed 2px black;
      
   }
  
   .item{
    
      display: flex;
      align-items: center;
    
  
   }

 





  </style>
