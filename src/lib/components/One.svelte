<script lang="ts">
 import { getContext } from "svelte";
 import { CONTEXT } from "./Parent.svelte";

 const { func } = getContext(CONTEXT) as any;
</script>

<div>
    tse
    <button on:click={func}>One</button>
</div>
