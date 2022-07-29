<script>
  import { Router } from 'svelte-router-spa'
  import { routes } from './routes.js'
</script>

<Router {routes} />

<style>
	:global(:target) {

	background-color: papayawhip;}
</style>
