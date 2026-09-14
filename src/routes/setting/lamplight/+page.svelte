<script>
  import DownloadButton from "$lib/components/DownloadButton.svelte"
  import italyMap from "$lib/maps/Fantasy Italy.png?enhanced"
  import townMap from "$lib/maps/Little Lamplight.png?enhanced"
</script>

<svelte:head>
  <title>The Town of Little Lamplight</title>
</svelte:head>

<h1>The Town of Little Lamplight</h1>

<DownloadButton url="Opening_game_overview.docx">Download the overview (.docx)</DownloadButton>

<p>Sixty leagues west of the free city Trieste, Little Lamp Light sits at the tip of a north flowing inlet off the Adriatic Sea.  Its west bank holds a garrison of troops from the Holy Roman empire. Captain Ippolita Sforza, commander of The Order of the Golden Fleece, said to be the great grandson of Phillip the Great, commands here. Its east bank holds another garrison, controlled by the Ottoman Empire, Admiral Hayreddin Barbarossa at its head.</p>

<enhanced:img src={italyMap} alt="Map of 1400s Italy showing the fictional location of Little Lamplight" />

<p><a href={italyMap} class="underline text-blue-900">Open full-size Italy map</a></p>

<p>The docks have opened this day and many a trading vessel sits in the inlet waiting its turn to off load. War ships from both factions sit calmly along each bank, a truce hangs over from the winter and thus far has held on into spring. Sailors from both factions can be seen watching casually as the trading ships come and go.</p>

<p>As ships dock, a compliment of Roman troops looks over the cargo, carefully selecting the 10% tithe from each vessel and offloading the trade goods into wagons for transport back to the garrison. Frustrated captains look on, hoping that the eyes of the Roman inspectors will overlook some of the more valuable cargo.</p>

<enhanced:img src={townMap} alt="A map of the town of Little Lamplight" />

<p><a href={townMap} class="underline text-blue-900" >Open full-size Little Lamplight map</a></p>

<p>In town, not a soul stands still. Full of nervous energy that only comes after a long hard winter ends, the townsfolk seem joyous and eager to greet the sunshine. Fruit and Vegetable stands are packed full of roots and tubers as well as the remains of last year's citrus, squash, cabbage and stew vegetables. Lines form down the main square, as most people have not had such for months, having lived off of salted meats and fish through the winter. Only the wealthy had enough stores to last them until spring.</p>

<p>Entire flocks of sheep, goats, and pigs are herded around town. Horses are off loaded as well, most of which get taken directly to the Roman garrison.</p>

<p>A small detachment of Roman troops can be found wandering the town keeping an eye out for trouble, but no one actually expects trouble today. Children run amok, winter's cork has finally been pulled, and spring time laughter and merriment flows from their smiling faces. Mothers barely trying to rein them in as no words spoken today will be able to hold them back.</p>

<p>At the Northern most tip of the town sits the Wayward (marked on the map by <b>&#128971;</b>), a three-story manor home with over thirty rooms. It houses children new born to age 16 -- orphans from the war -- many of these children coming from tragedy. The home has its own school, infirmary, workshop and stables. Children there are expected to learn to read and write, as well as pick up a trade. All children of walking age are expected to contribute in some way.</p>

<p>10 acres of land sit around the Wayward, used primarily for planting and grazing. The Wayward exists primarily because of its self-sufficiency. It even has its own green house were they successfully grow cucumbers and turnips year-round.</p>

<p>For Changelings in Little Lamp Light, the Wayward is ground central. Although the Wayward takes in children from the war it is simply a cover, its actual purpose is to facilitate the escape, and rehabilitation, of Changelings back into the real world. Not all changelings in Little Lamp Light stay at the Wayward, but all present are expected to support the Wayward's efforts.</p>

<p>Many Changelings, especially those who are older, live outside of the Wayward and support the Wayward's efforts buy providing a 10% tribute of their income. Older Changelings can be found doing all manner of jobs. Some work the ships, others own shops or have jobs in town. Some even are part of the factions that surround the town. No matter their ideals, no matter their background, the Wayward brings them together through community and protection.</p>
