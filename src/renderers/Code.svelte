<script>
  import { Highlight } from 'svelte-highlight'
  import atlas from 'svelte-highlight/src/styles/atlas'
  import {
    c,
    python,
    django,
    javascript,
    ruby,
    go,
    rust,
    shell,
    css,
    scss,
    yaml,
    json,
  } from 'svelte-highlight/src/languages'

  const LANGUAGES = {
    c: c,
    python: python,
    django: django,
    javascript: javascript,
    ruby: ruby,
    go: go,
    rust: rust,
    shell: shell,
    css: css,
    scss: scss,
    yaml: yaml,
    json: json,
  }

  export let lang
  export let text
</script>

<svelte:head>
  {@html atlas}
</svelte:head>

<Highlight code={text} language={LANGUAGES[lang]} />
