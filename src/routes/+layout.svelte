<script lang="ts">
    let { children } = $props();
</script>

<nav>
  <a href="/">Home</a>
  <a href="/setting">Setting</a>
  <a href="/maps">Hedge Maps</a>
  <a href="/rules">House Rules</a>
  <a href="/creation">Character Creation</a>
</nav>

{@render children()}

<footer class="text-xs">
  Copyright &copy; 2026 Dan Morell. Website by Paige Andrews of Level Nest Software.
</footer>
