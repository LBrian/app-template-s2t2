<script lang="typescript">
  import { onMount } from 'svelte';

  let count: number = 0;
  onMount(() => {
    const interval = setInterval(() => count++, 1000);
    return () => {
      clearInterval(interval);
    };
  });
</script>

<div class="App">
  <header>
    <img src="/logo.svg" class="App-logo" alt="logo" />
    <p>Edit <code>src/App.svelte</code> and save to reload.</p>
    <p>Page has been open for <code>{count}</code> seconds.</p>
    <p>
      <a
        class="App-link"
        href="https://svelte.dev"
        target="_blank"
        rel="noopener noreferrer"
      >
        Learn Svelte
      </a>
    </p>
  </header>
</div>

<style type="text/postcss">
  :global(body) {
    @apply m-0;
    font-family: Arial, Helvetica, sans-serif;
  }
  .App {
    @apply text-center text-xl;
  }
  .App code {
    @apply bg-red-200 px-1 py-2 rounded font-bold;
  }
  .App p {
    @apply m-2;
  }

  .App header {
    @apply bg-white text-black flex flex-col items-center justify-center min-h-screen;
  }
  .App-link {
    @apply text-red-600;
  }
  .App-logo {
    height: 36vmin;
    @apply animate-pulse mb-12 pointer-events-none;
  }
</style>
