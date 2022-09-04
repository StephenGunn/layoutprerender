<nav>
    <a href="/">home page</a>
</nav>
<hr>
<h2>
    Select a fake episode with prerender set to true:
</h2>
<ul>
    {#each Array(10) as episode, index}
        <li>
            <a href="/episodes-{index+1}">Episode #{index+1}</a>
        </li>
    {/each}
</ul>
<hr>
<h2>
    Select a fake episode with prerender not set at all:
</h2>
<ul>
    {#each Array(10) as episode, index}
        <li>
            <a href="/noprerender-{index+1}">No Prerender Episode #{index+1}</a>
        </li>
    {/each}
</ul>
<hr>
<slot></slot>