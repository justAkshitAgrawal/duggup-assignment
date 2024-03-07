<script>
	export let href = '/';
	export let imgSrc = '';
	export let label = '';
</script>

<a class="flex items-center gap-2" {href}>
	<img src={imgSrc} alt="Logo" class="" />
	<h1 class="text-sm font-medium text-[#4D4D4D] hover:text-black">
		{label}
	</h1>
</a>
