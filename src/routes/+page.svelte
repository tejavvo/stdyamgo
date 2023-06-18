<script>
    import Navbar from "$lib/nav.svelte";
    import Welcome from "$lib/welcome.svelte";
    import Slider from "$lib/slider.svelte";
</script>

<Navbar/>
<div style="padding: 0px 128px;">
    <Welcome user="ADMIN"/>
    <Slider/>
</div>