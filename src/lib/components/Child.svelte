<script lang="ts">
 export let mode = "string"

 import One from "./One.svelte"
 import Two from "./Two.svelte"
 import Three from "./Three.svelte"
</script>

{#if mode === "one"}
    <One />
{:else if mode === "two"}
    <Two />
{:else}
    <Three />
{/if}
