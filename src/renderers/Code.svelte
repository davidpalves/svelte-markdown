<script>
  import { HighlightAuto } from "svelte-highlight";

  export let lang
  export let text
</script>

<HighlightAuto code={text} />
