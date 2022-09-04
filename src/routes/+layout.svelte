<nav>
    <a href="/">home page</a>
</nav>
<hr>
<h2>
    Episodes: /episode-[number]/+layout.server.ts "prerender = true"
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
    Episodes: /noprerender-[number]/+layout.server.ts "prerender not set"
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