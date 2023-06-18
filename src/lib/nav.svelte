<script>
    export let links = ["Home", "Share", "Our Socials", "About"]
</script>

<div class="nav-bar">
    <img src="%sveltekit.assets%/favicon.png" alt="[ LOGO ]"/>
    <span>·</span>
    {#each links.reverse() as link}
      {#if link == "Home"}
        <a href="/">{link}</a>
      {:else}
        <a href="#{link.toLowerCase().replaceAll(" ", "-")}">{link}</a>
      {/if}
      <span>·</span>
    {/each}
</div>
<hr class="solid">
  
<style>
    .nav-bar {
      margin: 0;
      padding: 10px 125px;
      font-family: Alice;
      overflow: hidden;
    }
  
    .nav-bar a, span, img{
      color: #000000;
      text-align: center;
      padding: 14px 28px;
      text-decoration: none;
      font-size: 28px;
    }
  
    .nav-bar a, span {
      float: right;
    }
  
    .nav-bar img {
      float: left;
    }

    hr {
        background: #a6a6a6;
        border: 0;
        height: 1px;
    }
</style>
  