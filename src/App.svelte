<script>
  import { Router } from "svelte-navigator";
  import Navigator from "./components/Navigator.svelte";
  import 'material-icons/iconfont/material-icons.css';
  import ServerBanner from "./assets/server-banner.png";
</script>

<main>
  <Router primary={false}>
    <Navigator />
  </Router>
</main>

<style>
  main {
    display: flex;
    flex-direction: column;
    flex-grow: 1;
  }
</style>
