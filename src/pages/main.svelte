<script>

import Typewriter from 'svelte-typewriter'
 import Orbit from '../components/orbit.svelte';
import Card from "../components/skill_card.svelte";
import Projects from '../components/projects.svelte';
import About from '../components/About.svelte'
</script>


<div class="holder">
  <div class="lottie float">
    <lottie-player src="https://assets9.lottiefiles.com/packages/lf20_gljfnvqz.json"
      background="transparent" 
       speed="2"  
       style=" min-width:200px;min-height:500px ;width: 70%; height: 70%;"  
       loop  autoplay>
    </lottie-player>
</div> 
  
  <div class="intro">
<div class="intro_text">
   Hi !
</div>
<div class="intro_text">
   I Am <span style="color:red">Vishwa</span>
 </div>

 <div class="intro_text">
   
    {"<>"} 
    <Typewriter cascade loop interval={50}>
       
         <span style="color:#44aa8d">
           
            <div >Mobile App</div>
         </span>
         <span style="color:#ea7577">
           
            <div >Front End </div>
         </span>
         <span>
            <div >Web App </div>
         </span>
    </Typewriter>
    Developer
    {"</>"}
  </div>
  </div>
 
<div>
    
   
</div>

</div>



<div class="skills">
  <div class="orbit">
    <Orbit/>
  </div>
</div>

<div>
  <Card></Card>
</div>
<div>
  <Projects/>
</div>
<div>
  <About/>
</div>

<style>

.holder{
    display: flex;
    justify-content: space-between;
    padding:20px;
    /* Created with https://www.css-gradient.com */
transition: 1s linear;;

}
  .intro{
    padding:10px;
    background: #FFFFFF;
background: -webkit-radial-gradient(center, #FFFFFF, #ebebeb);
background: -moz-radial-gradient(center, #FFFFFF, #ececec);
background: linear-gradient(ellipse at center, #FFFFFF, #C4C4C4);
border-radius: 10px;
transition: 1s linear;;
height: 60%;


  }
  .intro_text{
    text-align:left;
    font-size: 3.5vh;
    font-weight: bold;
    margin:0px 20px 0px 20px ;
    
    
}

.lottie{
    display: flex;
 
    width:100%;
    min-width:100px;
   text-align: center;
  justify-content: center;
  align-items: center;
}

.float{
  animation:float 2s linear infinite
}

@keyframes 
float{
  0% { transform: translate(0,  -140px); }
    50%  { transform: translate(0, -135px); }
    100%   { transform: translate(0,-140px); }
}
.skills{
  display: flex;
  justify-content: center;
  margin-top:-35%;
 
}


span{
    color:rgb(37, 134, 219)
}


@media (min-width: 780px) {
  .holder{
    display: flex;
    justify-content: space-between;
    padding:40px;
    /* Created with https://www.css-gradient.com */

border-radius: 10px;;
border-radius: 100px;
}

.intro{
    width:100%;
    height:50%;
   margin-top: 5%;
   margin-left:10%;
 
}

.intro_text{
    text-align:center;
    font-size: 32px;
    font-weight: bold;
    font-family: 'Patrick Hand'
}

.skills{
  display: flex;
  justify-content: center;
  margin-top:0;
  margin-left:-10%
}

}



</style>