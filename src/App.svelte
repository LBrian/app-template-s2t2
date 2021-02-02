<script lang="typescript">
  import { onMount } from "svelte";

  let count: number = 0;
  onMount(() => {
    const interval = setInterval(() => count++, 1000);
    return () => {
      clearInterval(interval);
    };
  });
</script>

<div class="App">
  <header class="App-header">
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

<style>
  :global(body) {
    margin: 0;
    font-family: Arial, Helvetica, sans-serif;
  }
  .App {
    @apply text-center;
    @apply text-xl;
  }
  .App code {
    @apply bg-red-200;
    @apply px-1;
    @apply py-2;
    @apply rounded;
    @apply font-bold;
  }
  .App p {
    @apply m-2;
  }

  .App-header {
    @apply bg-white;
    @apply text-black;
    @apply flex;
    @apply flex-col;
    @apply items-center;
    @apply justify-center;
    min-height: 100vh;
  }
  .App-link {
    @apply text-red-600;
  }
  .App-logo {
    height: 36vmin;
    pointer-events: none;
    margin-bottom: 3rem;
    @apply animate-pulse;
  }
</style>
