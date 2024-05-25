<script lang="ts">
    import '$lib/css/main.css';
    import Nav from '$lib/components/Nav.svelte';
</script>

<header >
    site header
</header>

<main>
    <div class="content">
        <Nav/>
    </div>
    <div class="content">
        <slot>404</slot>
    </div>
</main>

<footer>
    site footer
</footer>

<style>
    main {
        display: grid;
        grid-template-rows: 2;
    }
</style>