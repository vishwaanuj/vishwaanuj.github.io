<script >
  

  import Main from './pages/main.svelte';
  import MediaQuery from "./components/Media_Q.svelte";
</script>

<ion-content>
  <MediaQuery query="(max-width: 600px)" let:matches>
    {#if matches}
    <Main/>

    {:else}

    <div class="noGo float">
      <div class="float">
        <h1> 🛸 </h1>
      </div>
    <div>
      <h1 >Please Use Phone To View</h1>
    </div>
     
    </div>
       
    {/if}
  </MediaQuery>

</ion-content>

<style>
  :root {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
      Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }

ion-content{
/* Created with https://www.css-gradient.com */
background: #d09393;
background: -webkit-radial-gradient(center, #FFFFFF, #C4C4C4);
background: -moz-radial-gradient(center, #FFFFFF, #C4C4C4);
background: radial-gradient(ellipse at center, #FFFFFF, #C4C4C4);
}

.noGo{

display:flex;
justify-content: center;
flex-direction: column;
align-items: center;
color:white;
background-color: black;
border-radius: 30px;
margin-top:25vh
}


  @media (min-width: 480px) {
 
  }

  .float{
  animation:float 4s cubic-bezier(0.39, 0.575, 0.565, 1) infinite
}

    @keyframes 
float{
  0% { transform: translate(0,  10px); }
    50%  { transform: translate(0, 20px); }
    100%   { transform: translate(0,10px); }
}
</style>
