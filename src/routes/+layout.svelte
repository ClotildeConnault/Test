<script lang="ts">
    import { onMount, type Snippet } from "svelte";
    import type { LayoutData } from "./$types";
    import "../app.css";
    import Navbar from "$lib/fragment/Navbar/Navbar.svelte";
    import Footer from "$lib/fragment/Footer/Footer.svelte";

    let { data, children }: { data: LayoutData; children: Snippet } = $props();
    let hasScrolled = $state(false);

    onMount(() => {
        window.addEventListener("scroll", handleScroll);
        return () => window.removeEventListener("scroll", handleScroll);
    });

    function handleScroll(this: Window, ev: Event) {
        hasScrolled = window.scrollY > 0;
    }
</script>

<Navbar scrolled={hasScrolled} />
<div class="min-h-[90vh] flex flex-col">
    {@render children()}
</div>
<Footer />
