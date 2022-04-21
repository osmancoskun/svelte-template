<script>
  import { onMount } from "svelte";
  export let id;
  export let type = "primary";
  export let inverse = false;
  export let flat = false;
  export let disabled;
</script>

<button on:click {disabled} {id} class={type} class:inverse class:flat>
  <slot />
</button>
