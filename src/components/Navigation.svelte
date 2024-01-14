<script lang="ts">
	import Icon from "@iconify/svelte";
</script>

<!-- Instagram-like tailwind responsive navigation bar -->
<!-- It should be on the bottom of the page -->
<!-- It should have these icons: Home, Explore, Create, Inbox, Profile -->

<div
	class="fixed bottom-0 left-0 right-0 flex items-center bg-white dark:bg-[#000] border-t border-gray-300 p-4 gap-4 justify-center"
>
	<a href="#home" class="text-xl font-bold text-black dark:text-white md:mr-6">
		<Icon icon="octicon:home-24" class="w-8 h-8" />
	</a>
	<a
		href="#explore"
		class="text-xl font-bold text-black dark:text-white md:mr-6"
	>
		<Icon icon="material-symbols:explore-outline" class="w-8 h-8" />
	</a>
	<a
		href="#create"
		class="text-xl font-bold text-black dark:text-white md:mr-6"
	>
		<Icon icon="mdi:plus-box-outline" class="w-8 h-8" />
	</a>
	<a href="#inbox" class="text-xl font-bold text-black dark:text-white md:mr-6">
		<Icon icon="mdi:email-outline" class="w-8 h-8" />
	</a>
	<a href="#profile" class="text-xl font-bold text-black dark:text-white">
		<Icon icon="mdi:account-outline" class="w-8 h-8" />
	</a>
</div>

<style lang="css">
</style>
