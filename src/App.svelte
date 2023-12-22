<script>
  import Router from 'svelte-spa-router';

  import Header from './lib/components/Header.svelte';
  import Footer from './lib/components/Footer.svelte';

  import Home from './lib/pages/Home.svelte';
  import Portfolio from './lib/pages/Portfolio.svelte';
  import Contact from './lib/pages/Contact.svelte';
  import NotFound from './lib/pages/NotFound.svelte';

  const routes = {
    "/": Home,
    "/portfolio": Portfolio,
    "/contact": Contact,
    "404-not-found": NotFound
  }
  
</script>

<Header />

<Router {routes} />

<Footer />