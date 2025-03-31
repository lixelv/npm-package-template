<script lang="ts">
    import { add } from "$lib/index.js"
    import { writable } from "svelte/store"

    const first = writable(1)
    const second = writable(2)

    $: sum = add($first, $second)
</script>

<input type="text" bind:value={$first}>
<input type="text" bind:value={$second}>
<p>{sum}</p>