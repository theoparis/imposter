<script lang="ts">
	import Icon from "@iconify/svelte";

	export let post = {
		profilePicture:
			"https://yt3.ggpht.com/6SUvLvQ6tJ8l6PAS3Y9OdsN7l-VVXVCsBhYqBcfvpfogaScX-3PoHVqq4mgbutsX-l-miiYgVA=s48-c-k-c0x00ffffff-no-rj",
		username: "juxtopposedme",
		content: "https://www.youtube.com/watch?v=GtffucAmM78",
	};
</script>

<div class="w-[468px] h-full flex flex-col justify-center items-center">
	<div class="flex justify-between items-center gap-4 w-full h-12">
		<div class="flex items-center gap-2">
			<div class="w-12 h-12 flex justify-center items-center">
				<div
					class="bg-gradient-to-tr from-yellow-400 to-pink-500 w-9 h-9 rounded-full flex justify-center items-center"
				>
					<div class="bg-white w-8 h-8 rounded-full p-1">
						<img
							src={post.profilePicture}
							alt="profile picture"
							class="w-full rounded-full"
						/>
					</div>
				</div>
			</div>
			<h1 class="text-base font-bold text-black dark:text-white">
				{post.username}
			</h1>
		</div>
		<div class="flex items-center">
			<Icon
				icon="mdi:dots-horizontal"
				class="w-6 h-6 text-black dark:text-white"
			/>
		</div>
	</div>

	<!-- Post content -->
	<div class="w-full h-full flex flex-col">
		<iframe
			class="w-full h-96"
			src="https://www.youtube.com/embed/GtffucAmM78?si=L9RjpYdQAQ73eCS5"
			title="YouTube video player"
			frameborder="0"
			allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
			allowfullscreen
		></iframe>
	</div>

	<!-- Post actions -->
	<div class="w-full h-12 flex justify-between items-center">
		<div class="flex justify-start items-center gap-4">
			<Icon
				icon="mdi:heart-outline"
				class="w-6 h-6 text-black dark:text-white"
			/>
			<Icon
				icon="iconamoon:comment"
				class="w-6 h-6 text-black dark:text-white"
			/>
			<Icon icon="tabler:send" class="w-6 h-6 text-black dark:text-white" />
		</div>
		<div class="flex justify-end items-center gap-4">
			<Icon
				icon="mdi:bookmark-outline"
				class="w-6 h-6 text-black dark:text-white"
			/>
		</div>
	</div>
</div>
