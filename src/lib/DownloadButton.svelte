<script>
  import { Download } from "@lucide/svelte"

  let { url, children } = $props()
</script>

<a href={url} class="bg-green text-white font-bold py-2 px-4 my-4 rounded inline-flex items-center transition-colors">
  <Download size={20} style="margin-right: 4px;" />
  <span>{@render children()}</span>
</a>

<style>
  a:hover {
    background-color: var(--bg-primary-dark);
  }
</style>
