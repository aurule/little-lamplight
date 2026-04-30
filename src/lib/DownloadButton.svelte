<script>
    import { Download } from "@lucide/svelte"

    let { url, children } = $props()
</script>

<a href="%sveltekit.assets%/Opening game overview.docx" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded inline-flex items-center">
    <Download size={20} style="margin-right: 4px;" />
    <span>{@render children()}</span>
</a>
