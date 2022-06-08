<script>

export let name;
export let des;
export let tech=[];
export let title;
</script>
<div class="project_name float">
    <img src={name} alt=""/>
    <div class="title">{title}</div>
  </div>
  <div class="project_des">
    {des} <br/>
   <div class="badges">
    {#each tech as i}
    
    <img class="badge" alt="" src={i}/>
  
    {/each}
   </div>
   
   
  </div>


  <style>
span{
  background-color: white;
  font-weight: 600;
}
img{
      margin:20px;
      width:30vw;
      height:25vh;
      border-radius: 10px;
      border:dashed 2px black;
      
   }
   .project_des{
  background-color: white;
  border-radius: 10px;
  padding:5px;
  font-family: 'Patrick Hand';
}

   .project_name{
  display: flex;
      align-items: center;
      flex-direction: column;
}
   .title{
     background-color: aliceblue;
     padding:5px;
     border-radius: 10px;
     font-weight: bold;
     
   }

   .float{
  animation:float 3s linear infinite
}


.badge{
    height:20px;
    width:20px;border:none;
    padding:0
}


.badges{
    display: flex;
    justify-content: left;
    width:50%
}
@keyframes 
float{
  0% { transform: translate(0,  0px); }
    50%  { transform: translate(0, -10px); }
    100%   { transform: translate(0,0px); }
}
  </style>