<div class="navbar bg-base-100 shadow-md">
  <div class="navbar-start">
  </div>
  <div class="navbar-center">
    <a href="/" class="p-2 btn btn-ghost">Home</a>
    <div class="megamenu max-sm:megamenu-vertical items-center justify-center" id="my-megamenu-1" popover>
      <span class="megamenu-active"></span>

      <button popovertarget="a1">Setting</button>
      <div id="a1" popover>
        <ul class="menu">
          <li><a href="/setting/lamplight">Little Lamplight</a></li>
          <li><a href="/setting/hedge">The Hedge</a></li>
        </ul>
      </div>

      <button popovertarget="a2">Pledges</button>
      <div id="a2" popover>
        <ul class="menu">
          <li><a href="/pledges/freehold">The Freehold Pledge</a></li>
          <li><a href="/pledges/worksheet">Pledge Building Worksheet</a></li>
        </ul>
      </div>

      <button popovertarget="a3">Rules</button>
      <div id="a3" popover>
        <ul class="menu">
          <li><a href="/rules/house-rules">House Rules</a></li>
          <li><a href="/rules/cheat-sheet/combat">Combat cheat Sheet</a></li>
          <li><a href="/rules/growth">Character Growth</a></li>
          <li><a href="/rules/creation">Character Creation</a></li>
        </ul>
      </div>
    </div>
  </div>
  <div class="navbar-end"></div>
  <button class="btn sm:hidden" popovertarget="my-megamenu-1">Menu</button>
</div>
