<script>
  import Item from "./Item.svelte";
  import Main from "./Main.svelte";
  //get url path
  const path = window.location.pathname;
  console.log(path);
  console.log(window.location.href)
  //console window.location.href after #/
  const url = window.location.href.split('#/')[1];
  //remove after ?
  const url2 = url.split('?')[0];
  console.log(url2);
</script>

{#if url2 == 'item'}
  <Item/>
{:else}
  <Main/>
{/if}

<style>
	:global(:target) {

	background-color: papayawhip;}
</style>
