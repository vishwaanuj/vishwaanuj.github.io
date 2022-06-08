<script>
    import Carousel from 'svelte-carousel'
    import DocturePoly from "./DocturePoly.png"
    import Nebiro from "./nebiro.png"
    import Jananya from "./jananya.png"
    let carousel; // for calling methods of the carousel instance
 
  </script>
  
  <Carousel


>

<div class="item float">
    <img src={DocturePoly} alt=""/>
    <div>DocturePoly</div>
</div>
<div class="item float">
    <img src={Nebiro} alt=""/>
    <div>Nebiro</div>
</div>
<div class="item float">
    <img src={Jananya} alt=""/>
    <div>Jananya</div>
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
      flex-direction: column;
  
   }

   .float{
  animation:float 3s linear infinite
}

@keyframes 
float{
  0% { transform: translate(0,  0px); }
    50%  { transform: translate(0, -5px); }
    100%   { transform: translate(0,0px); }
}
  </style>
