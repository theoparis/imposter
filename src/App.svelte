<script lang="ts">
	import Icon from "@iconify/svelte";
	import Navigation from "./components/Navigation.svelte";
	import Post from "./components/Post.svelte";

	let page = window.location.hash.slice(1) || "home";

	window.onhashchange = () => {
		page = window.location.hash.slice(1) || "home";
	};
</script>

<div
	class="w-full h-screen bg-gray-300 dark:bg-[#000] flex flex-col justify-center items-center"
>
	{#if page === "home"}
		<!-- Instagram post placeholders -->
		<div class="w-full h-full flex flex-col justify-center items-center">
			<div class="w-[468px] h-full grid grid-cols-1 gap-4">
				{#each Array(9) as i}
					<Post />
				{/each}
			</div>
		</div>
	{/if}

	<Navigation />
</div>
