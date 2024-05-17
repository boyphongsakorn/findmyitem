<script>
  import Item from "./Item.svelte";
  import Main from "./Main.svelte";
  //get url path
  const path = window.location.pathname;
  console.log(path);
  console.log(window.location.href)
  let url;
  let urlfinal;
  try {
    //console window.location.href after #/
    url = window.location.href.split('#/')[1];
    urlfinal = url.split('?')[0];
  } catch (error) {
    urlfinal = 'main';
  }
</script>

{#if urlfinal == 'item'}
  <Item/>
{:else}
  <Main/>
{/if}

<style>
	:global(:target) {

	background-color: papayawhip;}
</style>
