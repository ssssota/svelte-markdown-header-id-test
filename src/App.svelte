<script lang="ts">
	import SvelteMarkdownBefore from 'svelte-markdown-before';
	import SvelteMarkdownAfter from 'svelte-markdown-after';
	export let source = '# test\n\n## test\n';
</script>

<div>
<textarea rows="10" bind:value={source} />
</div>

before:
<div>
<SvelteMarkdownBefore {source} />
</div>

after:
<div>
<SvelteMarkdownAfter {source} />
</div>
