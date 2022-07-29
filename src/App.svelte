<script>
  //get url
  const url = new URL(window.location.href);
  //get path from url
  const path = url.pathname;
  import Item from "./Item.svelte";
</script>

  <main>
    {#if (path === "/")}
    test
    {/if}
    {#if (path === "/item")}
    <Item />
    {/if}
  </main>

<style>
	:global(:target) {

	background-color: papayawhip;}
</style>
