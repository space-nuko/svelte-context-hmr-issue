<script context="module" lang="ts">
 export const CONTEXT = {}
</script>

<script lang="ts">
 import { setContext } from "svelte";
 import Child from "./Child.svelte"

 let mode = "one"
 let state = 25;

 function func() {
     console.warn(`Function called! ${state++}`)
     if (mode == "one")
         mode = "two"
     else if (mode == "two")
         mode = "three"
     else
         mode = "one"
 }

 setContext(CONTEXT, {
     func
 })
</script>

<div>
    Test {state}

    <Child {mode} />
    <Child {mode} />
    <Child {mode} />
</div>
