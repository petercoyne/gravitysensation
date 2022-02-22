<script>
	import Header from '$lib/Header.svelte'
	import Logo from '$lib/Logo.svelte'
	import DiscordButton from '$lib/DiscordButton.svelte'
	import Download from '$lib/Download.svelte'
	import Tab from '$lib/Tab.svelte'
	import TabLink from '$lib/TabLink.svelte'
	import Box from '$lib/Box.svelte'
	
	let currentTab = "Features"
</script>

<Header style="page">
	<Logo align="left" size="w-36"/>
	<DiscordButton/>
</Header>

<div class="m-8 lg:max-w-4xl lg:mx-auto">
	<div id="summary" class="flex items-stretch gap-8 lg:gap-12">
		<div class="hidden sm:block rounded-3xl overflow-hidden object-cover">
			<img src="/images/tm/cover-vertical.webp" alt="Tricky Machines" class="hidden sm:block rounded-3xl max-h-[700px]">
		</div>
		<div class="flex flex-col py-8 lg:py-12">
			<h1 class="text-4xl mb-4">Tricky Machines</h1>
			<img src="/images/tm/cover-mobile.webp" alt="Tricky Machines" class="sm:hidden my-4 rounded-xl"/>
			<p class="grow opacity-80 leading-7 sm:text-sm md:text-base">Tricky Machines is a physics game with a built-in vehicle editor and
				map maker. Create your own scenarios or choose from hundreds
				of community made challenges.</p>
			<hr class="my-8 grow border-gs-blue opacity-30"/>
			<div class="flex gap-4">
				<Download kind="steam" limit="max-h-18" url="https://store.steampowered.com/app/1495380/Tricky_Machines/"/>
				<Download kind="apple" limit="max-h-18" url="https://apps.apple.com/us/app/tricky-machines/id1536951057"/>
				<Download kind="google" limit="max-h-18" url="https://play.google.com/store/apps/details?id=com.gravitysensation.trickymachines2"/>
			</div>
		</div>
	</div>
	
	<ul id="tab-bar" class="mt-6 mb-8 flex sm:text-xl md:text-2xl border-b gsborder justify-center sm:justify-start">
		<TabLink bind:currentTab tabName="Features"/>
		<TabLink bind:currentTab tabName="Screenshots"/>
		<TabLink bind:currentTab tabName="Videos"/>
	</ul>

	<Tab bind:currentTab tabName="Features">
		<Box heading="Design your own vehicles">
			<div class="flex items-center flex-col sm:flex-row">
				<div>
					<img src="/images/tm/vehicles1.webp" alt="selection of drivable vehicles"/>
				</div>
				<div>
					<img src="/images/tm/vehicles2.webp" alt="selection of drivable vehicles"/>
				</div>
			</div>
			<p class="mt-6 text-sm opacity-70"><b>Modify</b> any of the dozens of available vehicles, or <b>build</b> your own from scratch!</p>
		</Box>
		<div class="flex flex-col sm:flex-row mt-8 gap-8">
			<Box heading="Rewind Time">
					<div class="flex-1 flex items-center">
						<img src="/images/tm/rewind.webp" alt="rewind"/>
					</div>
					<p class="mt-6 text-sm opacity-70">Drive your best self with unlimited rewind.</p>
			</Box>
			<Box heading="Advanced Map Editor">
				<div class="flex flex-1 gap-4">
					<div>
						<img src="/images/tm/editor1.webp" alt="editor screenshot"/>
					</div>
					<div>
						<img src="/images/tm/editor1.webp" alt="editor screenshot"/>
					</div>
				</div>
				<p class="mt-6 text-sm opacity-70">Create a new world to explore, from the ground up.</p>
			</Box>
		</div>
	</Tab>
	<Tab bind:currentTab tabName="Screenshots">
		<p>Coming soon!</p>
	</Tab>
	<Tab bind:currentTab tabName="Videos">
		<div class="flex flex-col sm:flex-row gap-8">
			<iframe class="aspect-video w-full sm:w-1/2" src="https://www.youtube.com/embed/X6-wg3PZQj8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
			<iframe class="aspect-video w-full sm:w-1/2" src="https://www.youtube.com/embed/fJM2v5xsqOw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
		</div>
	</Tab>
</div>