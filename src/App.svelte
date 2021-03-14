<script lang="ts">
  import { Router, Route } from 'svelte-routing';
  import Home from './pages/Home.svelte';
  import NotFound from './pages/NotFound.svelte';
  import Broadcasts from './pages/Broadcasts.svelte';

  export let url: string;
  url = '';
</script>

<style lang="scss">
  :global(.container) {
    width: 80%;
    max-width: 1280px;
    margin: auto;
    @media (max-width: 1024px) {
      width: 100%;
    }
  }
</style>

<Router {url}>
  <Route path="/">
    <Home />
  </Route>
  <Route path="broadcasts" component={Broadcasts} />
  <Route component={NotFound} />
</Router>
