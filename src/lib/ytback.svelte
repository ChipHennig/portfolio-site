<script>
	export let id;
	import { onMount } from 'svelte';

	onMount(async () => {
		const module = await import('youtube-background');
		new VideoBackgrounds('[data-vbg]');
	});
</script>

<div data-vbg="https://www.youtube.com/watch?v={id}" />
