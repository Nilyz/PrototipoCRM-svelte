<script>
  import svelteLogo from './assets/svelte.svg'
  import viteLogo from '/vite.svg'
  import Splash from './screens/Splash.svelte'
  import Login from './screens/Login.svelte'
  import { Router, Route, link } from "svelte-routing"; // Importar el enrutador
</script>

<Router>
  <Route path="/" component={Splash} />
  <Route path="/login" component={Login} />
</Router>

<style>

</style>