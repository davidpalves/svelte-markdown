<script>
  import { Highlight } from "svelte-highlight";
  import python from "svelte-highlight/src/languages/python";
  import atlas from "svelte-highlight/src/styles/atlas";

  export let lang
  export let text
</script>


<svelte:head>
  {@html atlas}
</svelte:head>


<Highlight code="{text}" language={python}/>
