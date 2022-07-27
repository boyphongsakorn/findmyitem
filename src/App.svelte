<script>
  import { Router, Route, Link } from "svelte-navigator";
  import Item from "./Item.svelte";
</script>

<Router>
  <!--header>
    <h1>My site</h1>

    <nav>
      <Link to="/">Home</Link>
      <Link to="about">About</Link>
      <Link to="blog">Blog</Link>
    </nav>
  </header-->

  <main>
    <Route path="/item" component={Item} />

    <Route path="/">
      <h3>Home</h3>
      <p>Home sweet home...</p>
			<p>
				Check out the <Link to="/about#digital">digital heading</Link>, a heading with an <code>id </code> of “digital”
			</p>
    </Route>

    <Route>
      <h3>Default</h3>
      <p>No Route could be matched.</p>
    </Route>
  </main>
</Router>

<style>
	:global(:target) {

	background-color: papayawhip;}
</style>
