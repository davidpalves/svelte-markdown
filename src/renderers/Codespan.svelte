<script>
  import { HighlightAuto } from "svelte-highlight";
  import atlas from "svelte-highlight/src/styles/atlas";

  export let raw
</script>


<svelte:head>
  {@html atlas}
</svelte:head>


<HighlightAuto code={raw.replace(/`/g, '')} />

