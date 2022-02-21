<script>
	export let name, image, description, url;
</script>
<div class="flex flex-col">
	<h2 class="text-3xl pb-4">{name}</h2>
	<div class="object-cover rounded-xl overflow-hidden aspect-video">
		<img src="/images/{image}" alt="{name}"/>
	</div>
	<p class="text-sm lg:text-md py-4 leading-6 opacity-70 grow">{description}</p>
	<a href="{url}" class="text-gs-blue underline">Learn More</a>
	<div class="flex pt-6 gap-2">
		<slot/>
	</div>
</div>