<script>
 import "../node_modules/materialize-css/dist/css/materialize.min.css";
 import "../node_modules/materialize-css/dist/js/materialize.min.js";
 import { Router, Route } from "svelte-routing";

 import Navbar from "./layouts/Navbar.svelte";

 //  Import Pages
 import Home from "./pages/Home.svelte";
 import About from "./pages/About.svelte";
 import Contact from "./pages/Contact.svelte";
</script>

<style>
</style>

<h1>HEllo</h1>
<Router>
  <Navbar/>
  <div class="container">
    <Route path="/" component="{Home}"/>
    <Route path="/about" component="{About}"/>
    <Route path="/contact" component="{Contact}"/>
  </div>
</Router>
