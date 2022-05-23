<svelte:head>
  <link href="https://fonts.googleapis.com/css?family=Source+Sans+Pro:200,300,400,600" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css?family=IBM+Plex+Mono:200,300,400,600" rel="stylesheet">
</svelte:head>


<script>
  import BetaBar from '../components/BetaBar.svelte';
  import NavBar from '../components/NavBar.svelte';
  import "../app.css";
</script>


<div class="body">
  <BetaBar/>
  <NavBar/>
  <div class="content">
    <slot />
  </div>
</div>

<style>
  .body {
    background: #11151B;
  }

  .content {
    @apply max-w-[998px];
    @apply m-auto;
  }
</style>
