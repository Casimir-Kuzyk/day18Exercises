<script lang="ts">
  import Counter from './lib/Counter.svelte'
  import AlertButton from './lib/AlertButton.svelte'
  import NameInput from './lib/NameInput.svelte'
  import NFTView from './lib/NFTView.svelte'
</script>

<main>
  <div>

  </div>

  <div class="card">
    <Counter />
  </div>

  <div class="card">
    <AlertButton />
  </div>

  <div class="card">
    <NameInput />
  </div>

  <div class="card">
    <NFTView />
  </div>
  <p>
    Check out <a href="https://github.com/sveltejs/kit#readme" target="_blank" rel="noreferrer">SvelteKit</a>, the official Svelte app framework powered by Vite!
  </p>

  <p class="read-the-docs">
    Click on the Vite and Svelte logos to learn more
  </p>
</main>

<style>
  .logo {
    height: 6em;
    padding: 1.5em;
    will-change: filter;
    transition: filter 300ms;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
  .logo.svelte:hover {
    filter: drop-shadow(0 0 2em #ff3e00aa);
  }
  .read-the-docs {
    color: #888;
  }
</style>
