<script>
  import {Router, Route} from "svelte-routing";
  import About from "./Pages/About.svelte";
  import Home from "./Pages/Home.svelte";

  export const url = "";
</script>

<main class="row">
  <Router {url}>
    <Route path="/" component="{Home}"/>
    <Route path="/about" component="{About}"/>
  </Router>
</main>
