<script>
	export let tabName, currentTab
</script>

<li class="p-4" class:link="{currentTab != tabName}" on:click={() => currentTab = tabName}><h4>{tabName}</h4></li>