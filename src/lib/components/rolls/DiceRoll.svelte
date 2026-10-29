<script lang="ts">
  import type { Snippet } from "svelte";

  interface RollProps {
    /**
     * The name of the roll
     */
    name: string

    /**
     * The attribute to use for the roll
     *
     * Or, the first part of the dice pool
     */
    attribute: string

    /**
     * Name of the skill to add to the roll
     *
     * Or, the second part of the dice pool
     */
    skill?: string

    /**
     * Name of the third part to add to the roll
     *
     * Often Mantle or Wyrd
     */
    other?: string

    /**
     * The action needed to make this roll
     */
    action?: string

    /**
     * A cost required for the roll
     */
    cost?: string

    /**
     * How much time must pass between each roll
     */
    interval?: string

    /**
     * How many successes need to be gathered to succeed
     */
    target?: string

    /**
     * Modifier components
     */
    children?: Snippet
  }

  let { name, attribute, skill, other, action, children, cost, interval, target }: RollProps = $props()

  let uid = $props.id()

  let pool = $derived([attribute, skill, other].filter(Boolean).join(" + "))
</script>

<div class="dice-roll" aria-labelledby={uid}>
  <div class="name" id={uid}>{name}</div>
  <div class="info"><span class="label">Dice Pool:</span> {pool}</div>
  {#if action}<div class="info"><span class="label">Action:</span> {action}</div>{/if}
  {#if cost}<div class="info"><span class="label">Cost:</span> {cost}</div>{/if}
  {#if interval}<div class="info"><span class="label">Interval:</span> {interval}</div>{/if}
  {#if target}<div class="info"><span class="label">Target:</span> {target}</div>{/if}

  {#if children}
    <table class="modifiers table table-zebra w-fit">
      <caption>Suggested Modifiers</caption>
      <thead>
        <tr><th>Mod</th><th>Situation</th></tr>
      </thead>
      <tbody>
        {@render children()}
      </tbody>
    </table>
  {/if}
</div>

<style>
  .dice-roll {
    border: 1px solid var(--green-bright);
    padding: 1rem;
    display: inline-block;
  }

  .name {
    font-weight: bold;
    font-size: 1.1rem;
    color: var(--green-bright);
    margin-bottom: 0.5rem;
  }

  .label {
    font-weight: bold;
    color: var(--color-gray-400);
  }

  caption {
    font-weight: bold;
    color: var(--color-gray-400);
    margin: 0.5rem 0 0.3rem 0;
  }
</style>
