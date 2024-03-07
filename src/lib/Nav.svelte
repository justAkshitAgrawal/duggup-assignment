<script>
	import NavItem from './NavItem.svelte';
	import CtaButton from './CTAButton.svelte';
	import * as DropdownMenu from '$lib/components/ui/dropdown-menu/index';
	import { ChevronDown, User, Settings, LogOut } from 'lucide-svelte';
</script>

<div
	class="mx-40 flex justify-between border-b-[0.5px] border-dotted border-[#525C69]/50 px-2 py-4"
>
	<a class="flex items-center gap-1" href="/">
		<img src="/Logo.svg" alt="Logo" class="logo" />
		<img src="/duggup.png" alt="Logo" class="logo" />
	</a>

	<div class="flex items-center gap-10">
		<NavItem href="/home" imgSrc="/home.svg" label={'Home'} />
		<NavItem href="/explore" imgSrc="/explore.svg" label={'Explore'} />
		<NavItem href="/learn" imgSrc="/learn.svg" label={'Learn'} />
		<CtaButton label={'Post'} imgSrc="/post.svg" />

		<div>
			<DropdownMenu.Root>
				<DropdownMenu.Trigger class="flex items-center gap-2">
					<img src="/krishna.svg" alt="Profile" class="rounded-full border border-black" />
					<p class="text-[20px] font-medium">Krishna Kiran</p>
					<ChevronDown size="18" />
				</DropdownMenu.Trigger>
				<DropdownMenu.Content>
					<DropdownMenu.Group>
						<DropdownMenu.Item class="flex items-center gap-2 ">
							<User size="14" />
							Profile
						</DropdownMenu.Item>
						<DropdownMenu.Item class="flex items-center gap-2">
							<Settings size="14" />
							Settings
						</DropdownMenu.Item>
						<DropdownMenu.Item class="flex items-center gap-2">
							<LogOut size="14" />
							Log Out
						</DropdownMenu.Item>
					</DropdownMenu.Group>
				</DropdownMenu.Content>
			</DropdownMenu.Root>
		</div>
	</div>
</div>
