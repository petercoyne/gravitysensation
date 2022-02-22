<script>
	export let heading;
</script>

<div class="p-8 rounded-xl bg-black bg-opacity-20 border border-gs-blue-light border-opacity-20 shadow-xl flex flex-col">
	<p class="text-sm font-bold uppercase opacity-90 mb-6">{heading}</p>
	<slot/>
</div>