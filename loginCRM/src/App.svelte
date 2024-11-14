<!-- App.svelte -->
<script>
  import Splash from './screens/Splash.svelte';
  import Login from './screens/Login.svelte';
  import { Router, Route } from "svelte-routing";
</script>

<Router>
  <Route path="/" component={Splash} />
  <Route path="/login" component={Login} />
</Router>
