<script lang="ts">
	import type { Snippet } from "svelte";
    import Icon from '@iconify/svelte';

    type Props = {
        children: Snippet;
        title: string;
        poste: string;
        more?: Snippet;
    };

    let { children, title, poste, more }: Props = $props();

    let showMore = $state(false);
</script>

<div class="relative border-l pl-5 ">
    <div class="absolute top-0 left-0 w-5 h-5 rounded-full bg-[#1e293b] -translate-x-1/2 -translate-y-1/2"></div>
    <div class="absolute top-0 left-0 w-5 h-5 rounded-full bg-[#009688] -translate-x-1/2 translate-y-1/2"></div>
    <h2 class="text-3xl font-bold text-[#009688]">{title}</h2>
    <p class="text-xl font-bold ">{poste}</p>
    <div class="mt-5">
        {@render children()}
    </div>

    {#if more}
        <button class="flex justify-center items-center gap-1 text-[#009688] hover:cursor-pointer hover:underline mt-5 w-full" onclick={() => showMore = !showMore}><Icon icon="akar-icons:arrow-down" class={showMore ? "rotate-180" : ""} />{showMore ? "Voir moins" : "Voir plus"}</button>
        <div class={showMore ? 'block' : 'hidden'} >{@render more()}</div>
    {/if}
</div>