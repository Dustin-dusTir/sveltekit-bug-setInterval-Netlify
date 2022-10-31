<script>
  import { onDestroy } from "svelte";

  let counter = 0;
  const interval = setInterval(() => (counter += 1), 1000);

  onDestroy(() => clearInterval(interval));
</script>

<h1>Welcome to SvelteKit</h1>
<p>
  Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation
</p>
