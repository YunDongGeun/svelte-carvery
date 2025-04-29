<script>
  import Router from 'svelte-spa-router'
  import Main from './pages/Main.svelte'
  import CarWashInfo from './pages/CarWashInfo.svelte';
  import { fromStore } from 'svelte/store';
  import NotFound from './pages/NotFound.svelte';
  import "./css/style.css"

  const routes = {
    '/':Main,
    '/carwashinfo':CarWashInfo,
    '*':NotFound
  }
</script>

<Router routes={routes}/>

<style>
</style>
