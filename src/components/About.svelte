<script>

    import SkillCard from "./skill_card.svelte";
    import Me from "./me.png"
    import { GithubIcon,TwitterIcon,YoutubeIcon,LinkedinIcon } from 'svelte-feather-icons'
  
</script>


<SkillCard desc="A little about me "/>

<div class="content">
 <div class="thumbnail float">
    <lottie-player src="https://assets5.lottiefiles.com/packages/lf20_ccdngwrd.json"  background="transparent"  speed="1"  style="width: 200px; height: 400px;"  loop  autoplay></lottie-player>
 </div>
<div class="about">
  Hey! 
  I am self taught coder with a degree in 
  Mechatronics and a passion for tinkering.
  Currently,residing at hyderabad(India).
  Have an awesome idea wanna discuss with some coffee?
  Catch me on my social links!
  see you soon!

  
</div>


</div>
<div class="social">
    
  <a href="https://www.linkedin.com/in/vishwa-anuj/">  <LinkedinIcon size="20"/></a> 
   <a  href="https://www.youtube.com/channel/UCRz1K769DEI0D5o-zy7hZBg"><YoutubeIcon size="20"/></a> 
   <a href="https://github.com/vishwaanuj"> <GithubIcon size="20"/></a>
   <a href="https://twitter.com/VishwaAnuj1"><TwitterIcon size="20" /></a>  
</div>
<style>
    .content{
        display: flex;
        justify-content: space-evenly;
        padding:2vw;
        margin-top: -2vh;
       
    }

   .thumbnail {
        height: 220px;
       
        width:150px;
        border-radius: 100px;
        background-color: aliceblue;
        display: flex;
        align-items: center;
    }
    .thumbnail{
        display: flex;
        align-items: center;
    }
    .about{
        font-family: 'Patrick Hand';
        padding:10px;
        margin:10px;
        display: flex;
        justify-content: center;
        text-align: center;
        background-color: white;
        border-radius: 10px;
        text-align: justify;
    }
a{color:white}
    .social{
        padding:10px;
        display: flex;
        justify-content: space-evenly;
        color:white
    }

    .float{
  animation:float 4s cubic-bezier(0.39, 0.575, 0.565, 1) infinite
}

    @keyframes 
float{
  0% { transform: translate(0,  10px); }
    50%  { transform: translate(0, 30px); }
    100%   { transform: translate(0,10px); }
}
</style>