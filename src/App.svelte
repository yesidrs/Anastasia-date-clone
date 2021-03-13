<script lang="ts">
  import { Router, Route } from 'svelte-routing';
  import Home from './pages/Home.svelte';
  import NotFound from './pages/NotFound.svelte';

  export let url: string;
  url = '';
</script>

<style>
  :global(.container) {
    width: 80%;
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
