<script>
  import { HighlightAuto } from "svelte-highlight";
  export let raw
</script>

<HighlightAuto code={raw.replace(/`/g, '')} />
