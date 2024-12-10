<script lang="ts">
  import { Router, Link, Route } from "svelte-routing";
  import Navbar from "./components/Navbar.svelte";
  import Footer from "./components/Footer.svelte";
  import Home from "./routes/Home.svelte";
  import Services from "./routes/Services.svelte";
  import About from "./routes/About.svelte";
  import Contact from "./routes/Contact.svelte";
  import Foundation from "./routes/Foundation.svelte";
  import NewsTicker from "./components/NewsTicker.svelte";
  

  export let url = "";
</script>

<Router {url}>
  <div class="min-h-screen flex flex-col">
    <NewsTicker/>
    <Navbar />
    
    <main class="flex-grow">
      <Route path="/" component={Home} />
      <Route path="/services" component={Services} />
      <Route path="/about" component={About} />
      <Route path="/contact" component={Contact} />
      <Route path="/foundation" component={Foundation} />
    </main>

    <Footer />
  </div>
</Router>