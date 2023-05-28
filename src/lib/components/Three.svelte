<script lang="ts">
 import { getContext } from "svelte";
 import { CONTEXT } from "./Parent.svelte";

 const { func } = getContext(CONTEXT) as any;
</script>

<div>
    asdsadijasd
    <button on:click={func}>Three</button>
</div>
