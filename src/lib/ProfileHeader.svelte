<script>
	import CtaButton from './CTAButton.svelte';
	import { ExternalLink, MoreHorizontal } from 'lucide-svelte';
</script>

<div class="mt-10 flex justify-center">
	<div class="max-w-5xl">
		<div class="flex items-center gap-10">
			<div class="flex flex-col items-center">
				<img
					src="/krishna.svg"
					class="size-[120px] rounded-full border-[5px] border-[#EAEFF5]"
					alt=""
				/>
				<h1 class="text-center text-[24px] font-bold text-[#4B5C6D]">
					Krishna
					<br />
					Kiran
				</h1>
			</div>
			<div>
				<div class="flex items-center gap-32">
					<p class="w-[585px] text-sm text-[#141618]">
						Co-Founder and CEO at Duggup - Social network for people in tech. Ex-Amazon Head of
						Engineering. I write hot-takes on building a business, shipping delightful products and
						accelerating product and career growth.
					</p>
					<div class="flex flex-col items-end">
						<img src="/Logo.svg" alt="" class="size-[36px] rounded-full" />
						<h3 class="mt-2 text-[16px] font-bold">Duggup</h3>
						<p class="text-[12px] text-[#7A9299]">Co-Founder and CEO</p>
					</div>
				</div>
				<div class="mt-4 flex items-center justify-between">
					<CtaButton label="Follow" ctaActive={true} />

					<div class="flex items-center gap-4">
						<div
							class="flex cursor-pointer items-center gap-1 text-[#4d4d4d] transition-all hover:text-black"
						>
							<p class="text-[14px]">My Website</p>
							<ExternalLink size="16" class="" />
						</div>
						<MoreHorizontal
							size="24"
							class="cursor-pointer text-[#4d4d4d] transition-all hover:text-black"
						/>
					</div>
				</div>
			</div>
		</div>
	</div>
</div>
