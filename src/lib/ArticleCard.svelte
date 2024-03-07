<script>
	export let className = '';
	export let imgSrc = '';
	export let articleTitle = '';
</script>

<div class={`w-[344px] cursor-pointer rounded-[12px] border  ${className}`}>
	<div>
		<img src={imgSrc} alt="Article" class="h-[136px] w-[344px] rounded-t-[12px] object-cover" />
		<div class="p-4">
			<h1 class="text-[14px] text-[#141618]">
				{articleTitle.length > 84 ? `${articleTitle.slice(0, 84)}...` : articleTitle}
			</h1>
		</div>
	</div>
</div>
