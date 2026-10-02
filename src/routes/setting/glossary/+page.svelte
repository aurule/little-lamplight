<svelte:head>
  <title>Glossary | Little Lamplight</title>
</svelte:head>

<p>The denizens of Little Lamplight use different terminology for things than what can be found in the <i>Changeling: The Lost</i> source books.</p>

<dl>
  <dt id="dein-tuffel">Dein Tuffel</dt>
  <dd>
    <span class="pronunciation">deen <em>two</em>-fell</span>
    <span class="part">noun</span>
    One of the fae lords, a Gentry.
  </dd>

  <dt id="fegefeur">Fegefeur</dt>
  <dd>
    <span class="pronunciation"><em>fay</em>-geh-foor</span>
    <span class="part">noun</span>
    Arcadia, the realm of the <a href="#dein-tuffel">dein tuffel</a>.
  </dd>

  <dt id="oath">Oath</dt>
  <dd>
    <span class="part">noun</span>
    A magically enforced agreement, typically a Pledge.
  </dd>

  <dt id="wechelkind">Wechelkind</dt>
  <dd>
    <span class="pronunciation"><em>vesh</em>-el-kind</span>
    <span class="part">noun</span>
    Changelings. Those few who escape the captivity of people taken by the <a href="#dein-tuffel">dein tuffel</a>.
  </dd>

  <dt id="wechselbalg">Wechselbalg</dt>
  <dd>
    <span class="pronunciation"><em>veck</em>-sell-balg</span>
    <span class="part">noun</span>
    Fetches. Humanoid imposters left in the place of a kidnapped mortal.
    <div class="note">A character must have at least Changeling Lore 3 to know about wechselbalg, or have had an in-character conversation where they were explained.</div>
  </dd>

  <dt id="vich">Vich</dt>
  <dd>
    <span class="pronunciation">vitch</span>
    <span class="part">noun</span>
    Witch. Common term for someone, like a changeling, who performs supernatural feats.
  </dd>
</dl>

<style>
  dt {
    font-weight: bold;
  }

  dd {
    margin-bottom: 1rem;
  }

  .pronunciation {
    display: inline-block;
    &:before {
      content: "[";
    }
    &:after {
      content: "]";
    }
    margin-right: 0.7rem;

    em {
      font-style: inherit;
      font-weight: bold;
    }
  }

  .part {
    display: inline-block;
    margin-right: 0.7rem;
    font-style: italic;
  }

  .note {
    font-size: 0.8rem;
    color: var(--color-gray-400);

    &:before {
      content: "Note: ";
      font-style: italic;
    }
  }
</style>
