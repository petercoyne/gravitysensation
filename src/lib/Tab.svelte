<script>
	export let tabName, currentTab;
</script>

<div class:hidden="{currentTab != tabName}">
	<slot/>
</div>