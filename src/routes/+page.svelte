<script>
	import { storable } from '$lib/storable.js';

	const ui = storable({ logo: 'square' });
</script>

<img src="https://svelte.dev/whos-using-svelte/{$ui.logo}.svg" alt />
<br />
<button on:click={() => ($ui.logo = 'nyt')}>Update to NYT</button>
