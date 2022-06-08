<script>
  import logo from './assets/svelte.png'
  import Counter from './lib/Counter.svelte'
  import Main from './pages/main.svelte';
  import Header from './components/header.svelte';
</script>

<ion-content>

<Main/>
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


  @media (min-width: 480px) {
 
  }
</style>
