<script lang="ts">
    import type { LayoutData } from '../../../.svelte-kit/types/src/routes/episode-noprerender-[number]/$types'
    export let data: LayoutData

</script>

<h1>Dynamic Test Episode #{data.number} - {data.episode.title} - not pre-rendered at +layout level</h1>
<nav>
    <a href="/episodes-{data.number}">Episode Home Page</a> | 
    <a href="/episodes-{data.number}/gallery">Episode #{data.number} Gallery</a>
</nav>
<hr>
<slot></slot>