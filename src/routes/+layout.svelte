<script>
    import '../styles/global.css'
    import Header from '$lib/Header.svelte';
</script>

<Header/>
<main>
    <slot /> <!--Page specific code-->
</main>