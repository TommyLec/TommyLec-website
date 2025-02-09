<script lang="ts">
	import { cn } from '$lib/utils';
    import Icon from '@iconify/svelte';
    let { title, icon, highlight = false } = $props();
</script>

<div class={cn("flex flex-col justify-center items-center  rounded-md p-4 w-32", highlight ? "bg-[#009688]/50" : "bg-slate-400/20")}>
    <Icon icon={icon} width="50" height="50" />
    <p class="text-sm mt-2">{title}</p>
</div>