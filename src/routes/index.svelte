<script>
	import Header from '$lib/Header.svelte'
	import Logo from '$lib/Logo.svelte'
	import DiscordButton from '$lib/DiscordButton.svelte'
	import HomeGrid from '$lib/HomeGrid.svelte'
	import Game from '$lib/Game.svelte'
	import Download from '$lib/Download.svelte'
</script>

<Header style="home">
	<Logo align="center" size="w-28"/>
	<DiscordButton/>
</Header>
<HomeGrid>
	<Game name="Tricky Machines"
		image="tm-home.webp"
		description="Tricky Machines is a physics game with a built-in vehicle editor and map maker. Create your own scenarios or choose from hundreds of community made challenges."
		url="/trickymachines/">
		<Download kind="steam" url="https://store.steampowered.com/app/1495380/Tricky_Machines/"/>
		<Download kind="apple" url="https://apps.apple.com/us/app/tricky-machines/id1536951057"/>
		<Download kind="google" url="https://play.google.com/store/apps/details?id=com.gravitysensation.trickymachines2"/>
	</Game>
	<Game name="Goofball Goals"
		image="goof-home.webp"
		description="Goofball Goals is a very happy soccer game with fully physically based character animation using interactive alive ragdolls in a destructible environment."
		url="http://www.gravitysensation.com/goofball/">
		<Download kind="windows" url="http://www.gravitysensation.com/goofball/Goofball_Setup.exe"/>
		<Download kind="apple" url="https://itunes.apple.com/us/app/goofball-goals/id913321161?ls=1&mt=8"/>
		<Download kind="google" url="https://play.google.com/store/apps/details?id=com.gravitysensation.igoof"/>
	</Game>
	<Game name="Tricky Truck"
		image="tt-home.webp"
		description="Test your parking skills with huge trucks. Drive through hard mountain roads. Fully physics based gameplay."
		url="http://www.gravitysensation.com/trickytruck/">
		<Download kind="windows" url="http://www.gravitysensation.com/trickytruck/Tricky_Truck_Setup.exe"/>
	</Game>
	<Game name="Sumotori Dreams"
		image="sumo-home.webp"
		description="Sumotori Dreams is a light hearted ragdoll game and screen saver, where two japanese wrestlers have to force the opponent to the ground."
		url="http://www.gravitysensation.com/sumotori/">
		<Download kind="steam" url="https://store.steampowered.com/app/1604240/Sumotori_Dreams_Classic"/>
		<Download kind="apple" url="https://itunes.apple.com/us/app/sumotori-dreams/id838455884?ls=1&mt=8"/>
		<Download kind="google" url="https://play.google.com/store/apps/details?id=com.gravitysensation.sumotori"/>
	</Game>
</HomeGrid>