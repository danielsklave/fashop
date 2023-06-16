<div class="mx-4 mb-8">
	<a class="card card-hover overflow-hidden" href="/#/item">
		<img src="https://source.unsplash.com/Q-72wa9-7Dg/400x800" class="w-full aspect-[4/3] rounded object-cover" alt="Post"> 
	</a>

	<br/>

	<div class="flex justify-between mx-2">
		<h3 class="mb-4">For you</h3>
		<a href="/"><small>See All</small></a>
	</div>
	<div class="flex gap-4">
		{#each [1,2,3] as i}
			<a class="card card-hover overflow-hidden" href="/#/item">
				<header><img src="https://source.unsplash.com/iIjResyhhW0/400x700" class="w-full aspect-[3/4] rounded object-cover" alt="Post"></header> 
				<footer><small>Example Outfit {i}</small></footer>
			</a>
		{/each}
	</div>

	<br/>

	<div class="flex justify-between mx-2">
		<h3 class="mb-4">Top Trends</h3>
		<a href="/"><small>See All</small></a>
	</div>
	<div class="flex gap-4">
		{#each [1,2,3] as i}
			<a class="card card-hover overflow-hidden" href="/#/item">
				<header><img src="https://source.unsplash.com/iIjResyhhW0/400x700" class="w-full aspect-[3/4] rounded object-cover" alt="Post"></header> 
				<footer><small>Example Outfit {i}</small></footer>
			</a>
		{/each}
	</div>
</div>