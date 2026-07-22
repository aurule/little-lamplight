<script lang="ts">
  import './layout.css';
  import Navigation from "./components/Navigation.svelte"
  import { setContext } from 'svelte';

  let { children } = $props();

  let width = $state(0)
  let isMobile = $derived(width < 768)
  setContext("isMobile", () => isMobile)
</script>

<svelte:window bind:innerWidth={width} />

<Navigation />

{@render children()}

<footer class="text-xs text-center" style="margin-top: 1rem;">Copyright © 2026 Dan Morell. Website by Paige Andrews of Level Nest Software.</footer>
