<nav>
    <a href="/">home page</a>
</nav>
<hr>
<h2>
    Select a fake episode:
</h2>
<ul>
    {#each Array(10) as episode, index}
        <li>
            <a href="/episodes-{index+1}">Episode #{index+1}</a>
        </li>
    {/each}
</ul>
<hr>
<slot></slot>