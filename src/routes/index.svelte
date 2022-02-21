<script>
	import Header from '$lib/Header.svelte'
	import Logo from '$lib/Logo.svelte'
	import DiscordButton from '$lib/DiscordButton.svelte'
	import HomeGrid from '$lib/HomeGrid.svelte'
	import HomeGame from '$lib/HomeGame.svelte'
	import HomeDownload from '$lib/HomeDownload.svelte'
</script>

<Header style="center">
	<Logo align="center" size="medium"/>
	<DiscordButton/>
</Header>
<HomeGrid>
	<HomeGame name="Tricky Machines"
		image="tm-home.webp"
		description="Tricky Machines is a physics game with a built-in vehicle editor and map maker. Create your own scenarios or choose from hundreds of community made challenges."
		url="/trickymachines/">
		<HomeDownload kind="steam" url="https://store.steampowered.com/app/1495380/Tricky_Machines/"/>
		<HomeDownload kind="apple" url="https://store.steampowered.com/app/1495380/Tricky_Machines/"/>
		<HomeDownload kind="google" url="https://store.steampowered.com/app/1495380/Tricky_Machines/"/>
	</HomeGame>
	<HomeGame name="Goofball Goals"
		image="goof-home.webp"
		description="Goofball Goals is a very happy soccer game with fully physically based character animation using interactive alive ragdolls in a destructible environment."
		url="/trickymachines/">
		<HomeDownload kind="windows" url="https://store.steampowered.com/app/1495380/Tricky_Machines/"/>
		<HomeDownload kind="apple" url="https://store.steampowered.com/app/1495380/Tricky_Machines/"/>
		<HomeDownload kind="google" url="https://store.steampowered.com/app/1495380/Tricky_Machines/"/>
	</HomeGame>
	<HomeGame name="Tricky Truck"
		image="tt-home.webp"
		description="Test your parking skills with huge trucks. Drive through hard mountain roads. Fully physics based gameplay."
		url="/trickymachines/">
		<HomeDownload kind="windows" url="https://store.steampowered.com/app/1495380/Tricky_Machines/"/>
	</HomeGame>
	<HomeGame name="Sumotori Dreams"
		image="sumo-home.webp"
		description="Sumotori Dreams is a light hearted ragdoll game and screen saver, where two japanese wrestlers have to force the opponent to the ground."
		url="/trickymachines/">
		<HomeDownload kind="windows" url="https://store.steampowered.com/app/1495380/Tricky_Machines/"/>
		<HomeDownload kind="google" url="https://store.steampowered.com/app/1495380/Tricky_Machines/"/>
	</HomeGame>
</HomeGrid>