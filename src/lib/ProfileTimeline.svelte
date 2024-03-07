<script>
	import ArticleCard from './ArticleCard.svelte';
	import { ChevronUp } from 'lucide-svelte';
</script>

<div class="flex items-center justify-center">
	<div class="mt-4 w-full max-w-5xl">
		<div class="relative ml-[70px] h-[110vh] w-2 border-r border-dotted border-[#778FB1]">
			<div
				class="absolute left-1/2 top-[15vh] h-4 w-4 -translate-x-1 -translate-y-1/2 rounded-full border-[3px] border-[#0066FF] bg-white"
			>
				<p class="absolute right-20 w-full -translate-y-1 text-nowrap text-[12px] text-[#7A9299]">
					Dec 2023
				</p>
				<ArticleCard
					className="absolute left-20 -translate-y-20"
					articleTitle="No amount of technology can convert a bad story into a good story."
					imgSrc="/steve.jpg"
				/>
				<ArticleCard
					className="absolute left-[450px] -translate-y-20"
					articleTitle="Most people don't have original ideas. Here is how Sam Altman pushes himself to have unpopular ideas."
					imgSrc="/sam.jpg"
				/>
			</div>

			<ChevronUp
				size="24"
				color="#778FB1"
				class="absolute left-1/2 top-[35vh] -translate-x-[0.45rem] -translate-y-1/2 "
			/>

			<div
				class="absolute left-1/2 top-[45vh] h-4 w-4 -translate-x-[0.6rem] -translate-y-1/2 rounded-full border-[10px] border-[#0066FF] bg-white p-1"
			>
				<div class="absolute -bottom-12 right-10 flex w-40 flex-col items-end">
					<img src="/Logo.svg" alt="" class="size-[48px] rounded-full" />
					<h1 class="text-[16px] font-bold">Duggup</h1>
					<p class="text-[12px] text-[#7A9299]">San Francisco Bay Area</p>
					<p class="text-right text-[12px] text-[#7A9299]">Joined <br /> Nov 2023</p>
				</div>
				<div class="absolute -bottom-0 left-20 flex w-60 flex-col items-start">
					<h1 class="text-[20px] font-bold">Co-Founder and CEO</h1>
					<p class="text-[12px] text-[#7A9299]">Full-time Remote</p>
				</div>
			</div>

			<div
				class="absolute left-1/2 top-[65vh] h-4 w-4 -translate-x-1 -translate-y-1/2 rounded-full border-[3px] border-[#0066FF] bg-white"
			>
				<p class="absolute right-20 w-full -translate-y-1 text-nowrap text-[12px] text-[#7A9299]">
					Dec 2022
				</p>
				<ArticleCard
					className="absolute left-20 -translate-y-20"
					articleTitle={`Startup Lesson I am reflecting. Don't build for the \"average person".`}
					imgSrc="/laptop.jpg"
				/>
				<ArticleCard
					className="absolute left-[450px] -translate-y-20"
					articleTitle="Your biggest regrets at 80 will be acts of omission."
					imgSrc="/map.png"
				/>
			</div>

			<ChevronUp
				size="24"
				color="#778FB1"
				class="absolute left-1/2 top-[85vh] -translate-x-[0.45rem] -translate-y-1/2 "
			/>

			<div
				class="absolute left-1/2 top-[95vh] h-4 w-4 -translate-x-[0.6rem] -translate-y-1/2 rounded-full border-[10px] border-[#0066FF] bg-white p-1"
			>
				<div class="absolute -bottom-12 right-10 flex w-40 flex-col items-end">
					<img src="/better.svg" alt="" class="size-[48px] rounded-full" />
					<h1 class="text-[16px] font-bold">BetterUp</h1>
					<p class="text-[12px] text-[#7A9299]">San Francisco Bay Area</p>
					<p class="text-right text-[12px] text-[#7A9299]">Joined <br /> Sep 2022</p>
				</div>
				<div class="absolute -bottom-0 left-20 flex w-60 flex-col items-start">
					<h1 class="text-[20px] font-bold">VP Engineering</h1>
					<p class="text-[12px] text-[#7A9299]">Full-time</p>
				</div>
			</div>
		</div>
	</div>
</div>
