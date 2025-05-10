<script lang="ts">
    import type { Snippet } from "svelte";

    interface ICard {
        color?: string;
        background: string;
        children: Snippet;
    }
    let { color = "#fab900", background, children }: ICard = $props();
</script>

<div
    class="relative select-none flex overflow-hidden border-t-8 border-l-8 border-blue-900 w-fit h-80 flex-1 mt-7 items-center justify-center-safe text-white text-4xl"
>
    <img
        src={background}
        alt="background"
        class="absolute top-0 left-0 h-80 w-full object-cover"
    />
    <div class="h-full w-full bg-black/20 z-10 absolute top-0 left-0"></div>
    <p class="select-none text-center z-20">{@render children()}</p>
</div>
