<script>
    import "../app.pcss";
    import "../app.pcss";
    import Header from "./components/Header.svelte";
    import Footer from "./components/Footer.svelte";

</script>

<div class="min-h-screen flex flex-col">
 <Header/>
  <main class="m-14 flex-grow">
   <slot />
  </main>
 <Footer />
</div>







