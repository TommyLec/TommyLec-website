<script lang="ts">
	import Icon from '@iconify/svelte';
</script>

<div class="mb-28">
	<h2 class="text-center text-3xl font-bold text-[#009688]">Contactez-moi</h2>

	<div class="flex flex-col items-center justify-center gap-4 mt-5">
		<a
			class="flex w-fit items-center gap-2 rounded-md border-3 border-[#009688] px-4 py-2 text-[#009688] hover:cursor-pointer hover:bg-[#009688] hover:text-white"
			href="mailto:tommy.lecourt@gmail.com"
		>
			<Icon icon="mdi:email" width="20" height="20" /> tommy.lecourt@gmail.com
		</a>
		<span
			class="flex w-fit items-center gap-2 rounded-md border-3 border-[#009688] px-4 py-2 text-[#009688]"
		>
			<Icon icon="mdi:phone" width="20" height="20" /> 06 59 08 01 70
		</span>
		<a
			class="flex w-fit items-center gap-2 rounded-md border-3 border-[#009688] px-4 py-2 text-[#009688] hover:cursor-pointer hover:bg-[#009688] hover:text-white"
			href="https://www.linkedin.com/in/tommy-lecourt/"
			target="_blank"
		>
			<Icon icon="mdi:linkedin" width="20" height="20" /> tommy.lecourt
		</a>
	</div>
</div>
