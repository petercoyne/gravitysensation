<script>
	export let style;
</script>

{#if style == "home"}
	<div class="flex flex-col p-24 pb-8 items-center gap-12">
		<slot/>
	</div>
{:else}
	<div class="flex lg:max-w-4xl lg:mx-auto gap-8 mx-8 pt-16 pb-4 sm:pb-6 mb-8 items-center justify-between border-b gsborder">
		<slot/>
	</div>
{/if}