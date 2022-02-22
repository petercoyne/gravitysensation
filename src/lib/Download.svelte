<script>
	export let kind, url, limit;
</script>

{#if limit}
<a href="{url}" class="shadow-lg">
	<img src="/images/dl-{kind}.webp" alt="Download on {kind}" class="{limit}"/>
</a>
{:else}
<a href="{url}" class="shadow-lg">
	<img src="/images/dl-{kind}.webp" alt="Download on {kind}" class="max-h-16 md:max-h-10 lg:max-h-12"/>
</a>
{/if}