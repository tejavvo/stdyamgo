<script>
    var items = ["Notes", "Find", "Blog", "Chat", "Profile"];
</script>

<div class="scroll-container">
    {#each items as item}
        <a href="{item.toLowerCase().replaceAll(" ", "-")}"><img src="/images/{item}.png" alt="{item}" width="auto" height="600"></a>
    {/each}
</div>    

<style>
    div.scroll-container {
        overflow: auto;
        white-space: nowrap;
        padding: 10px;
    }
    
    div.scroll-container img {
        padding: 10px;
    }
</style>
