<script>
  import DownloadButton from "$lib/components/DownloadButton.svelte"
</script>

<svelte:head>
  <title>Pledge Building Worksheet | Little Lamplight</title>
</svelte:head>

<h1>Pledge Building Worksheet</h1>

<DownloadButton url="/Pledge_Building_Worksheet.pdf">Download Worksheet (.pdf)</DownloadButton>

<h2>Tips</h2>

<p>The points added and removed by various pledge aspects must add to zero.</p>
<p>Pledges should include boons, tasks, and sanctions of similar severity.</p>
<p>Some aspects add to the cost of enacting the pledge. These must be paid when the pledge is sworn.</p>
<p>Each character is limited to a single oath of any given type, except Vows.</p>
<p>Any extra penalties only apply to Changeling parties.</p>
<p>Sanctions must be chosen ahead of time between changelings. They can be declared in the moment against mortals.</p>
<p>Sanctions last as long as the pledge that was broken. Against a mortal, you can invest a point of Willpower to extend the sanction for another such interval, but it counts against your total number of Vow pledges.</p>
<p>You can add someone to a pledge by gathering all the sworn and each spending a willpower while the new member spends the invocation cost of the pledge. Fealty pledges work differently.</p>

<h2>Steps to Build a Pledge</h2>

<p>These can be used alongside the worksheet to help remember what you need. Page references are given for the core <i>Changeling: The Lost</i> book, 1st edition, 2007 printing.</p>

<ol class="list-decimal list-inside">
  <li>Name the parties</li>
  <li>
    Pick the type of oath
    <table class="table w-fit ml-6">
      <thead>
        <tr>
          <th>Oath</th>
          <th>Description</th>
          <th>Additional Penalties</th>
          <th>Page</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>Vow</th>
          <td>The common oath. Can have Wyrd + 3 sworn at a time.</td>
          <td>None</td>
          <td>176</td>
        </tr>
        <tr>
          <th>True Name, Obscured</th>
          <td>Sworn on the name you share with your fetch</td>
          <td>Weakened the next time you encounter your fetch. Lose all resistance to fetch powers, have 0 Defense, subtract Wyrd from all rolls. Your fetch knows you're weak.</td>
          <td>176</td>
        </tr>
        <tr>
          <th>True Name, Unsullied</th>
          <td>Sworn on your true name</td>
          <td>Must have no fetch. All Vows are broken and you suffer the sanctions of every one of them. All formerly bound know you broke an oath on your True Name.</td>
          <td>177</td>
        </tr>
        <tr>
          <th>Name of the Keeper</th>
          <td>Swear on your own Keeper's name. All parties must be Changelings.</td>
          <td>Keeper knows where you are and can add your Wyrd to their rolls against you sometime within the next year and a day.</td>
          <td>177</td>
        </tr>
        <tr>
          <th>Name of a Higher Power</th>
          <td>Swear on the divine</td>
          <td>Lose all willpower points. Take -1 penalty on next Clarity degeneration roll.</td>
          <td>177</td>
        </tr>
        <tr>
          <th>Mortal Emblem</th>
          <td>Swear on a connection to the mortal world</td>
          <td>Become ejected or excluded from the related organization. Roll degeneration check at 4 dice. Subtract -2 if the pledge was broken due to your life among the fae. Add +2 if it was broken while fulfilling a Virtue. Subract -2 if it was broken while fulfilling a Vice.</td>
          <td>177</td>
        </tr>
        <tr>
          <th>Seeming Emblem</th>
          <td>Swear on a symbol of your nature</td>
          <td>Lose a point of Wyrd. Cannot be sworn at Wyrd 1. Typically used by both parties if it's used at all.</td>
          <td>178</td>
        </tr>
        <tr>
          <th>Courtly Emblem</th>
          <td>Swear on a symbol of your Mantle</td>
          <td>Must have a Mantle or Court Goodwill merit. Lose all dots of Court Goodwill, or reduce Mantle by half. For one moon, members of the court can sense the broken oath.</td>
          <td>178</td>
        </tr>
        <tr>
          <th>Title Emblem</th>
          <td>Swear on a symbol of your Entitlement</td>
          <td>Lose the benefits of your entitlement until you gain a new point of Wyrd. All in the entitlement know you broke the oath.</td>
          <td>178</td>
        </tr>
        <tr>
          <th>Nemesis</th>
          <td>Swear on the symbol of another changeling</td>
          <td>Would-be nemesis must agree. Immediately suffer effects of the contract the Nemesis uses when the pledge is sworn, like a <a href="#pishogue">pishogue</a> sanction. Nemesis knows who broke the oath.</td>
          <td>178</td>
        </tr>
      </tbody>
    </table>
  </li>
  <li>
    Choose tasks
    <table class="table w-fit ml-6">
      <thead>
        <tr>
          <th>Task</th>
          <th>Rating</th>
          <th>Requirement</th>
          <th>Points</th>
          <th>Page</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th rowspan="3" class="w-3xs">
            Alliance
            <p class="font-normal">Rather like a combined Ban and Endeavor. Always applies to all parties.</p>
          </th>
          <td>Lesser</td>
          <td>A.k.a. the "peace pact". A simple pledge not to hinder one another.</td>
          <td>+0</td>
          <td>178</td>
        </tr>
        <tr>
          <td>Medial</td>
          <td>Expected to help each other as necessary. Willing to risk harm or inflict it, but death is too much.</td>
          <td>-2</td>
          <td>178</td>
        </tr>
        <tr>
          <td>Greater</td>
          <td>Expected to help each other despite torture or death.</td>
          <td>-3</td>
          <td>178</td>
        </tr>
        <tr>
          <th>Dreaming</th>
          <td>Medial</td>
          <td>May enter the dreams of another pledgebound and are obligated to do so.</td>
          <td>-2</td>
          <td>179</td>
        </tr>
        <tr>
          <th rowspan="3" class="w-3xs">Endeavor</th>
          <td>Lesser</td>
          <td>Rarely difficult to accomplish. Like frequently doing something that requires hardly any time or effort, or doing a single task that requires a small imposition. The task must not risk harm.</td>
          <td>-1</td>
          <td>179</td>
        </tr>
        <tr>
          <td>Medial</td>
          <td>Takes some effort to do. A constant activity that requires a small amount of time or effort, or a single task that is difficult or risks harm.</td>
          <td>-2</td>
          <td>179</td>
        </tr>
        <tr>
          <td>Greater</td>
          <td>An epic task. A constant activity that needs significant attention and effort, or a single task that is tremendously difficult or may result in death.</td>
          <td>-3</td>
          <td>179</td>
        </tr>
        <tr id="ensorcellment">
          <th>Ensorcellment</th>
          <td>Medial</td>
          <td>May only be performed by a changeling on behalf of a mortal. Invests one glamour in the mortal (spent when the pledge is sworn) which can be reclaimed with a touch, but this breaks the pledge. Counts as an equal <a href="#ensor-boon">Ensorcellment Boon</a> for the mortal, so Ensorcellment is self-balancing.</td>
          <td>-2</td>
          <td>179</td>
        </tr>
        <tr id="fealty">
          <th>Fealty</th>
          <td>Greater</td>
          <td>Must be sworn from a vassal to a freehold ruler. Always comes with the <a href="#vassalage">Vassalage boon</a> and the <a href="#banishment">Banishment sanction</a>. The ruler commits a <i>dot</i> of willpower to the pledge the first time it is sworn, but not for additional signers-on. The willpower returns if the ruler steps down voluntarily in a ceremony, but is lost if they are overthrown.</td>
          <td>-3</td>
          <td>180</td>
        </tr>
        <tr>
          <th rowspan="3" class="w-3xs">Forbiddance</th>
          <td>Lesser</td>
          <td>Don't do something that is easily avoided. An action that doesn't come up often, or and there is no difficulty in not doing it.</td>
          <td>-1</td>
          <td>180</td>
        </tr>
        <tr>
          <td>Medial</td>
          <td>Don't do something that's somewhat difficult to avoid. The action might come up more often, or avoiding it may be inconvenient.</td>
          <td>-2</td>
          <td>180</td>
        </tr>
        <tr>
          <td>Greater</td>
          <td>Don't so something that's very hard to avoid. The action might come up constantly, or be very difficult to avoid taking.</td>
          <td>-3</td>
          <td>180</td>
        </tr>
      </tbody>
    </table>
  </li>
  <li>
    Choose boons
    <table class="table w-fit ml-6">
      <thead>
        <tr>
          <th>Boon</th>
          <th>Rating</th>
          <th>Benefit</th>
          <th>Points</th>
          <th>Page</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>Adroitness</th>
          <td>Lesser</td>
          <td>Gain +1 bonus to all rolls of a single, named skill.</td>
          <td>+1</td>
          <td>180</td>
        </tr>
        <tr>
          <th rowspan="3" class="w-3xs">
            Alliance
            <p class="font-normal">Can only increase non-supernatural merits.</p></th>
          <td>Lesser</td>
          <td>Grant a mortal a new 1- or 2-dot merit, or increase an existing merit by 1 dot. Grant a supernatural creature a new 1-dot merit, or increase an existing merit by 1 dot.</td>
          <td>+1</td>
          <td>180</td>
        </tr>
        <tr>
          <td>Medial</td>
          <td>Grant a mortal a new 3- or 4-dot merit, or increase an existing merit by 2 dots. Grant a supernatural creature a new 2-dot merit, or increase an existing merit by 2 dots.</td>
          <td>+2</td>
          <td>181</td>
        </tr>
        <tr>
          <td>Greater</td>
          <td>Grant a mortal a new 5-dot merit, or increase an existing merit by 3 dots. Grant a supernatural creature a new 3-dot merit, or increase an existing merit by 3 dots.</td>
          <td>+3</td>
          <td>181</td>
        </tr>
        <tr id="ensor-boon">
          <th>Ensorcellment</th>
          <td>Medial</td>
          <td>Perceive seemings, miens, and other things of Wyrd and Glamour. Granted by the <a href="#ensorcellment">Ensorcellment boon</a>.</td>
          <td>+2</td>
          <td>181, 279</td>
        </tr>
        <tr>
          <th>Favor</th>
          <td>Any</td>
          <td>Perform an appropriately difficult task when asked in the future.</td>
          <td>+1 to +3</td>
          <td>181, 279</td>
        </tr>
        <tr>
          <th>Glamour</th>
          <td>Medial</td>
          <td>
            <p>From one changeling to another, this boon directly transfers glamour, either all at once or over time. The max total transferred is equal to the highest Wyrd of all participants. The max transferred at a time is equal to the <em>lowest</em> Wyrd of all participants. Glamour can be transferred over time at most once per week.</p>
            <p>From a mortal to a changeling, this boon grants one point of glamour at an interval, with no maximum total. The minimum interval is one day.</p>
          </td>
          <td>+2</td>
          <td>181</td>
        </tr>
        <tr>
          <th id="vassalage">Vassalage</th>
          <td>Greater</td>
          <td>Considered a member of the freehold and get its blessing while within its borders. Can only be granted by a pledge including the <a href="#fealty">Fealty task</a>.</td>
          <td>+3</td>
          <td>181</td>
        </tr>
      </tbody>
    </table>
  </li>
  <li>
    Choose sanctions
    <table class="table w-fit ml-6">
      <thead>
        <tr>
          <th>Sanction</th>
          <th>Rating</th>
          <th>Punishment</th>
          <th>Points</th>
          <th>Page</th>
        </tr>
      </thead>
      <tbody>
        <tr id="banishment">
          <th>Banishment</th>
          <td>Greater</td>
          <td>Must be pronounced by the freehold lord to take effect. Can be pronounced at <em>any time</em>. Any who owe fealty to that lord gains 1 Glamour for acting to harm the traitor within the freehold's borders. Killing the oathbreaker within the freehold grants glamour equal to the slain one's Wyrd.</td>
          <td>-3</td>
          <td>182</td>
        </tr>
        <tr>
          <th rowspan="3" class="w-3xs" id="lesser-curse">
            Curse
            <p class="font-normal">Curses of varying power stack: 2 <i>lessers</i> become a <i>medial</i>, and 3 <i>lessers</i> or 2 <i>medials</i> become a <i>greater</i>. The newly potent curse gets the longest duration of the stacked curses.</p></th>
          <td>Lesser</td>
          <td>May not re-roll 10s.</td>
          <td>-1</td>
          <td>182</td>
        </tr>
        <tr>
          <td>Medial</td>
          <td>Only succeed on a 9 or a 10.</td>
          <td>-2</td>
          <td>182</td>
        </tr>
        <tr>
          <td>Greater</td>
          <td>Only succeed on a 10. A roll with no successes becomes a Dramatic Failure, but you can spend 1 willpower to make it a regular failure.</td>
          <td>-3</td>
          <td>182</td>
        </tr>
        <tr>
          <th>Death</th>
          <td>Greater</td>
          <td>
            <p>Betrayed party loses a dot of willpower when the oath is broken, and the oathbreaker begins to die. Within days equal to the Wyrd of the wronged party (1 week for a betrayed mortal), the Wyrd will arrange a fatal accident.</p>
            <p>Genuine, uncoerced forgiveness lifts the doom and restores the dot of willpower</p>
          </td>
          <td>-3</td>
          <td>182</td>
        </tr>
        <tr>
          <th>Flaw</th>
          <td>Medial</td>
          <td>Gain a permanent flaw (see WoD 1e 217) within a week of breaking the oath. The flaw can be chosen beforehand or left up to the Wyrd.</td>
          <td>-2</td>
          <td>183</td>
        </tr>
        <tr>
          <th rowspan="3" class="w-3xs" id="pishogue">
            Pishogue
            <p class="font-normal">One or more contracts are activated when the pledge is sworn, with all costs paid, to a minimum of 1 glamour each. Takes effect with no resistance. The caster knows that the pact is broken.</p></th>
          <td>Lesser</td>
          <td>Suffer a 1- or 2-dot contract.</td>
          <td>-1</td>
          <td>183</td>
        </tr>
        <tr>
          <td>Medial</td>
          <td>Suffer a 3- or 4-dot contract, or two separate <i>lessers</i>.</td>
          <td>-2</td>
          <td>183</td>
        </tr>
        <tr>
          <td>Greater</td>
          <td>Suffer a 5-dot contract, or: 3 <i>lessers</i>, 1 <i>lesser</i> and 1 <i>medial</i>, or 2 <i>medials</i>.</td>
          <td>-3</td>
          <td>183</td>
        </tr>
        <tr>
          <th rowspan="5" class="w-3xs">
            Poisoning of Boon
            <p class="font-normal">Points always negate those of the boon that is poisoned.</p></th>
          <td>Adroitness</td>
          <td>Suffer a -1 to that skill.</td>
          <td rowspan="5">varies</td>
          <td>183</td>
        </tr>
        <tr>
          <td>Blessing</td>
          <td>A boosted merit loses points equal to what it had gained. If that brings it below the minimum rating for that merit, rolls formerly afftected by the merit suffer a <a href="#lesser-curse">lesser curse</a>.</td>
          <td>183</td>
        </tr>
        <tr>
          <td>Ensorcellment</td>
          <td>Fae things remain visible, but become terrifying. Nightmares cause a Resolve + Composure roll each week (-1 per week) to avoid gaining a new derangement. Must roll Resolve + Composure (-1 per week) when seeing fae things or react in great terror.</td>
          <td>183</td>
        </tr>
        <tr>
          <td>Favor</td>
          <td>Reverse debtor and owed.</td>
          <td>184</td>
        </tr>
        <tr>
          <td>Glamour</td>
          <td>Between changelings, the transfer is reversed. Between fae and changeling, the fae simply loses 1 point of glamour whenever they would have received one.</td>
          <td>184</td>
        </tr>
        <tr>
          <th rowspan="2" class="w-3xs">
            Vulnerability
            <p class="font-normal">The one betrayed is always allowed seek vengeance, even if normally prevented by another oath.</p></th>
          <td>Glamour</td>
          <td>Automatically fail opposed rolls against Contracts, and do not subtract anything from non-opposed activation rolls. Defense is 0 vs Contracts and Wyrd-based abilities, but not against normal attacks.</td>
          <td>-2</td>
          <td>184</td>
        </tr>
        <tr>
          <td>Violence</td>
          <td>Defense is 0. Attacks bypass all Contract or Wyrd-based bonuses to defense or armor.</td>
          <td>-2</td>
          <td>184</td>
        </tr>
      </tbody>
    </table>
  </li>
  <li>
    Choose duration
    <table class="table w-fit ml-6">
      <thead>
        <tr>
          <th>Duration</th>
          <th>Rating</th>
          <th>Definition</th>
          <th>Points</th>
          <th>Page</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>Day</th>
          <td>Lesser</td>
          <td>Exactly 24 hours. A casual oath.</td>
          <td>+1</td>
          <td>184</td>
        </tr>
        <tr>
          <th>Week</th>
          <td>Lesser</td>
          <td>Exactly 7 days to the hour</td>
          <td>+1</td>
          <td>184</td>
        </tr>
        <tr>
          <th>Moon</th>
          <td>Medial</td>
          <td>28 days. The shortest "serious" oath.</td>
          <td>+2</td>
          <td>184</td>
        </tr>
        <tr>
          <th>Season</th>
          <td>Medial</td>
          <td>Often sworn at a solstice or equinox. Outside those celestial events, spans 89 days.</td>
          <td>+2</td>
          <td>184</td>
        </tr>
        <tr>
          <th>Year and a Day</th>
          <td>Greater</td>
          <td>Exactly 366 days</td>
          <td>+3</td>
          <td>184</td>
        </tr>
        <tr>
          <th>Decade</th>
          <td>Greater</td>
          <td>Exactly 10 years and 10 days. Rarely sworn.</td>
          <td>+3</td>
          <td>184</td>
        </tr>
        <tr>
          <th>Lifelong</th>
          <td>Greater</td>
          <td>Invest a permanent dot of Willpower from one participant.</td>
          <td>+3</td>
          <td>184</td>
        </tr>
        <tr>
          <th>Generational</th>
          <td>Greater</td>
          <td>Invest a permanent dot of Willpower from one participant. Spans a number of generations equal to the Wyrd of the oathtaker who spends their willpower dot. Almost unheard-of. Onus passes to the children or sworn heirs of the participants.</td>
          <td>+3</td>
          <td>184</td>
        </tr>
      </tbody>
    </table>
  </li>
</ol>
