<script lang="ts">
    import type { PageData } from '../../../.svelte-kit/types/src/routes/episode-noprerender-[number]/$types'
    export let data: PageData
</script>

    <h2>Welcome to the index of episode #{data.number}</h2>

    {@html data.episode.body}
