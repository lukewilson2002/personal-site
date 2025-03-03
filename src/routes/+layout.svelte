<script lang="ts">
  import "../global.css";

  let { children } = $props();
</script>

<header>
  <nav>
    <a href="/">Home</a>
    <a href="/blog">Blog</a>
  </nav>  
</header>
<main>
  {@render children()}
</main>

<style>
  header {
    margin: 0 auto;
    padding: 0 1rem;
    max-width: var(--content-width);
  }

  nav {
    display: flex;
    gap: 1rem;
    padding-bottom: 1rem;
    border-bottom: 1px solid var(--border-color);
  }
</style>
