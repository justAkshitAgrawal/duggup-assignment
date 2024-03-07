<script>
	import { writable } from 'svelte/store';

	// Props
	export let label = 'Button'; // This will be updated from the parent component
	export let imgSrc = '';
	export let ctaActive = false;

	// Create a local writable store for label if it needs to be updated internally
	let internalLabel = writable(label);

	// Emit an event when the button is clicked
	function handleClick() {
		if (ctaActive) {
			internalLabel.update((n) => (n === 'Follow' ? 'Followed' : 'Follow'));
		}
	}
</script>

<button
	class="flex cursor-pointer items-center justify-center gap-2 rounded border-[0.5px] border-[#4D4D4D] px-6 py-1 text-sm text-[#4d4d4d] shadow-[0px_4px_0px_0px_rgba(77,77,77,1)] transition-all hover:translate-y-[3px] hover:shadow-none
      {ctaActive
		? ' hover:translate-y-[1px] hover:border-[#0066FF] hover:bg-[#0066FF] hover:text-white hover:shadow-[0px_2px_0px_0px_rgba(0,58,145,1)]'
		: ''}
    "
	on:click={handleClick}
>
	{#if imgSrc}
		<img src={imgSrc} alt="Logo" class="-ml-0.5" />
	{/if}
	<span>
		{$internalLabel}
		<!-- Use the local store's value -->
	</span>
</button>
