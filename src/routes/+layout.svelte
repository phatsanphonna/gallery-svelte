<script lang="ts">
    import "../app.css";
    import Navbar from "$lib/components/Navbar.svelte";
</script>

<Navbar />

<head>
    <link href="https://cdn.jsdelivr.net/gh/lazywasabi/thai-web-fonts@7/fonts/LINESeedSansTH/LINESeedSansTH.css" rel="stylesheet" />
</head>

<main class="container mx-auto pt-4">
    <slot />
</main>
