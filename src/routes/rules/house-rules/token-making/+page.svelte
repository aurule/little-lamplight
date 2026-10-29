<script lang="ts">
  import DiceRoll from "$lib/components/rolls/DiceRoll.svelte";
  import Modifier from "$lib/components/rolls/Modifier.svelte";
</script>

<svelte:head>
  <title>Making Tokens | Little Lamplight</title>
</svelte:head>

<h1>Making Tokens</h1>

<p>The <a href="/setting/glossary#wechelkind">wechelkind</a> of Little Lamplight are able to create their own tokens. Doing so requires an enormous amount of time and effort, but the results can be as powerful as any artefact bought at the goblin market.</p>

<h2>The Plans</h2>

<p>To make a token, you must first have a plan for how to do it. This plan can be a set of detailed instructions, an in-depth recipe, or a literal blueprint full of schematics.</p>

<p>Plans can potentially be purchased from goblins or other wechelkind, or discovered hidden in places throughout the hedge.</p>

<p>You can also create your own plans from scratch. Doing this requires an extended Intelligence + Occult roll, with a target of 5 successes per dot of the final token, and allowing one roll made per day.</p>

<DiceRoll
  name="Create a Token Plan"
  attribute="Intelligence"
  skill="Occult"
  target="5 successes / dot of the fininshed token"
  interval="1 day"
  >
</DiceRoll>

<h2>The Crafting Process</h2>

<p>With plan in hand, you can begin crafting your token. This is a very long process that requires dedication and a consistent infusion of glamour.</p>

<p>The crafting requires an extended Wyrd + Crafts roll. Your character should have some background in the type of crafting involved in the token, but you don't need a full specialty. The total successes needed is 25 per dot of the finished token. Each roll requires two weeks of work at 8 hours each day, and an expenditure of at least 1 glamour. The two-week interval is <em>not</em> affected by merits such as Brownie Boon: they can reduce the daily work hours instead.</p>

<p>Having a Workshop in a specialty relevant to the crafting at hand cuts the work time in half for that part of the token, meaning 1 week per roll instead of 2 weeks. Work with the STs to determine how much of the token can be done at this pace.</p>

<p>Failure on a crafting roll does not subtract from your total, nor does it ruin anything about the token. You simply don't make progress for that period of time.</p>

<DiceRoll
  name="Craft a Token"
  attribute="Wyrd"
  skill="Craft"
  target="25 successes / dot of the finished token"
  interval="2 weeks of 8 hour days"
  cost="1 glamour / roll"
  >
  <Modifier bonus={1} situation="Each additional glamour spent. You can only spend 5 glamour in total on token crafting each month." />
  <Modifier bonus={2} situation="Working 16+ hours each day. This can be reduced by merits like Brownie Boon." />
</DiceRoll>

<h2>Interruptions</h2>

<p>You can temporarily stop work on a token to see to other matters. As long as you resume crafting within 2 weeks, you can pick up right where you left off.</p>

<p>If you stop working for more than two weeks, all accumulated successes are lost as the glamour seeps out of the unfinished token.</p>
