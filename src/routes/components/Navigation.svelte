<script lang="ts">
  import { getContext } from "svelte";
  import { page } from "$app/state"
  import { DropdownMenu } from "bits-ui";
  import { ChevronDown, ChevronUp } from "@lucide/svelte";

  let isMobile: CallableFunction = getContext("isMobile")

  const links = new Map<string, string>([
    ["/", "Home"],
    ["/setting", "Setting"],
    ["/maps", "Maps"],
    ["/rules", "House Rules"],
    ["/characters", "Character Rules"],
  ])

  let current_path = $derived(page.url.pathname)
  let current_label = $derived(links.get(current_path))
  let open = $state(false)
</script>

{#if isMobile()}
  <DropdownMenu.Root bind:open>
    <DropdownMenu.Trigger class="w-5/6 min-w-50 mx-auto block">
      <nav class="current border rounded border-black bg-white p-1 m-3 flex gap-2 justify-center items-center block">
        {current_label}
        {#if open}
          <ChevronUp size={16} />
        {:else}
          <ChevronDown size={16} />
        {/if}
      </nav>
    </DropdownMenu.Trigger>
    <DropdownMenu.Portal>
      <DropdownMenu.Content class="w-5/6 min-w-50">
        <div class="border rounded border-black p-2 bg-white min-w-50">
          {#each links.entries() as [path, label] (path)}
            {#if current_path != path}
              <DropdownMenu.Item>
                <a class="block w-full" href={path}>{label}</a>
              </DropdownMenu.Item>
            {/if}
          {/each}
        </div>
      </DropdownMenu.Content>
    </DropdownMenu.Portal>
  </DropdownMenu.Root>
{:else}
  <nav class="border rounded border-black p-1 m-3 flex gap-4 justify-center">
    {#each links.entries() as [path, label] (path)}
      {#if current_path == path}
        <span class="current underline">{label}</span>
      {:else}
        <a href={path}>{label}</a>
      {/if}
    {/each}
  </nav>
{/if}

<style>
  .current {
    color: #008C45;
    cursor: default;
  }
</style>
