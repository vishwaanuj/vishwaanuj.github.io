<script>
import Python from './python.png'
import Svelte from './svelte.png'
import React from './react.png'
import Ionic from './ionic.png'
</script>



<div class="small_orbit rotate float">
<img src={Python} alt="" class="item rotate1 " style="bottom:0"/>
<img src={Svelte} alt="" class="item rotate1 " style="top:0;right:0"/>
<img src={React} alt="" class="item rotate1 " style="top:0;left:0"/>
<img src={Ionic} alt="" class="item " style="bottom:0;right:0"/>
</div>

<style>
.small_orbit{
  height:30vh;
  width:30vh;
  border-radius: 500px;
  border:dotted 2px white;


}
.item{
width:35px;
height:35px;
position: absolute;
border-radius: 200px;
background-color: white;
border:solid 1px black;
padding:20px;

}
.float{
  animation:float 2s linear infinite
}

@keyframes 
float{
  0% { transform: translate(0,  -140px); }
    50%  { transform: translate(0, -15px); }
    100%   { transform: translate(0,-140px); }
}

.rotate{
  animation: rotate 6.5s cubic-bezier(0.785, 0.135, 0.15, 0.86) infinite; 
}
@keyframes rotate{
  to{ transform: rotate(360deg); }
}

.rotate1{
  animation: rotate1 25s linear infinite; 
}
@keyframes rotate1{
  to{ transform: rotate(360deg); }
}
@media (min-width: 780px) {
  
  .small_orbit{
  height:300px;
  width:300px;
  border-radius: 500px;
  border:dotted 2px white;
}

.item{
width:70px;
height:70px;
position: absolute;
border-radius: 200px;
background-color: white;
}


}
</style>