<script lang="ts">
    import type { LayoutData } from '../../../.svelte-kit/types/src/routes/episode-noprerender-[number]/$types'
    export let data: LayoutData

</script>

<h1>Test Episode #{data.number} - {data.episode.title}</h1>
<nav>
    <a href="/episodes-{data.number}">Episode Home Page</a> | 
    <a href="/episodes-{data.number}/gallery">Episode #{data.number} Gallery</a>
</nav>
<hr>
<slot></slot>

<style>

</style>