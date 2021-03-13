<script>
  import { Router, Route } from 'svelte-routing';
  import Home from './pages/Home.svelte';
  import NotFound from './pages/NotFound.svelte';

  export let url = '';
</script>

<style>
  :global(.container) {
    width: 85%;
    max-width: 1280px;
    margin: auto;
  }
</style>

<Router {url}>
  <Route path="/">
    <Home />
  </Route>
  <Route component={NotFound} />
</Router>
