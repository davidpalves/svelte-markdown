<script>
  import { HighlightAuto } from "svelte-highlight";
  import atlas from "svelte-highlight/src/styles/atlas";

  export let lang
  export let text
</script>


<svelte:head>
  {@html atlas}
</svelte:head>


<HighlightAuto code="{text}" langtag="{true}"/>
