<script lang="ts">
 import { getContext } from "svelte";
 import { CONTEXT } from "./Parent.svelte";

 const { func } = getContext(CONTEXT) as any;
</script>

<div>
    <button on:click={func}>Two</button>
</div>
