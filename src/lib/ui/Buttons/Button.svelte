<script lang="ts">
    import { goto } from "$app/navigation";
    import type { Snippet } from "svelte";

    interface IButton {
        route: string;
        text?: string;
        variant?: "primary" | "secondary" | "tertiary";
        children?: Snippet;
    }

    let { route, text = "", variant = "primary", children = null } = $props();

    function navigate() {
        goto(route);
    }
</script>

<button onclick={navigate}
    class="px-4 py-2 border-3 border-white hover:border-blue-950 hover:text-blue-950 text-white text-xl duration-150 font-semibold"
>
    {#if text}
        {text}
    {:else if children}
        {@render children()}
    {/if}
</button>
