<script lang="ts">
    import Icon from '@iconify/svelte';
    let { title, img, href } = $props();
</script>

<div class="group min-w-56 min-h-42 rounded-xl overflow-hidden relative">
    <a href={href}>
        <div class="absolute object-cover w-full h-full -z-10 bg-[#009688]/20 transition-all backdrop-blur-xs group-hover:backdrop-blur-none"></div>
        <img src={img} alt={title} class="absolute object-cover w-full h-full -z-20 grayscale group-hover:grayscale-0 transition-all" />
        <div class="z-40 h-full flex flex-col justify-end p-2 text-white">
            <h2 class="text-2xl font-bold group-hover:opacity-0 transition-all">{title}</h2>
            <div class="flex items-center gap-1  group-hover:text-2xl transition-all">
                <span>Voir</span> <Icon icon="akar-icons:link-out" />
            </div>
        </div>
    </a>
</div>