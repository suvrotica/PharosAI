<script context="module" lang="ts">
  import { onMount } from 'svelte';
  import "@picocss/pico";
  let fontLoaded = false;

  onMount(async () => {
    const fontLink = document.createElement("link");
    fontLink.href = "https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap";
    fontLink.rel = "stylesheet";
    document.head.appendChild(fontLink);
    fontLoaded = true;
  });
</script>

<svelte:head>
  <style>
    body {
      font-family: 'Roboto', sans-serif;
    }
  </style>
</svelte:head>





  <main class="container">
    <article>
      <header> <nav>
        <nav>
          <ul>
            <li><strong>Pharos AI</strong></li>
          </ul>
          <ul>
            <li><a href="/">Home</a></li>
            <li><a href="/about">About</a></li>
            <li><a href="/contact">Contact</a></li>
          </ul>
       </header>
      <slot/>
      <footer>Pharos AI</footer>
    </article>
   
   
  </main>
  
 