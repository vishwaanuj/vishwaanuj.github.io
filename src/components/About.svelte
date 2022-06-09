<script>

    import SkillCard from "./skill_card.svelte";
    import Me from "./me.png"
    import { GithubIcon,TwitterIcon,YoutubeIcon,LinkedinIcon } from 'svelte-feather-icons'
  
</script>


<SkillCard desc="A little about me "/>

<div class="content">
 <div class="thumbnail float">
    <img  src={Me} alt=""/>
 </div>
<div class="about">
  Hey! 
  I am self taught coder with a degree in 
  Mechatronics and a passion for tinkering.
  Currently,residing at Hyderabad(India).
  Have an awesome idea wanna discuss with some coffee?
  Catch me on my social links!
  see you soon!

  
</div>


</div>
<div class="social">
    <a href="https://twitter.com/VishwaAnuj1"><TwitterIcon size="20" /></a>
   <a href="https://www.youtube.com/channel/UCRz1K769DEI0D5o-zy7hZBg"><YoutubeIcon size="20"/></a> 
   <a href="https://github.com/vishwaanuj"> <GithubIcon size="20"/></a>
   <a href="https://www.linkedin.com/in/vishwa-anuj/"><LinkedinIcon size="20"/></a> 
</div>
<style>
    .content{
        display: flex;
        justify-content: space-evenly;
        padding:2vw;
        margin-top: -2vh;
       
    }

   .thumbnail img{
        height: 120px;
        width:120px;
        border-radius: 100px;
    }
    .thumbnail{
        display: flex;
        align-items: center;
    }

    a{
        color:white
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

    .social{
        padding:10px;
        display: flex;
        justify-content: space-evenly;
        color:white
    }

    .float{
  animation:float 3s cubic-bezier(0.39, 0.575, 0.565, 1) infinite
}

    @keyframes 
float{
  0% { transform: translate(0,  0px); }
    50%  { transform: translate(0, -10px); }
    100%   { transform: translate(0,0px); }
}
</style>