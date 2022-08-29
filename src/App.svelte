<script>
  import Home from './pages/Home.svelte';
  import Rules from './pages/Rules.svelte';
  import Vote from './pages/Vote.svelte';
  import Staff from './pages/Staff.svelte';
  import Wiki from './pages/Wiki.svelte';
  import Support from './pages/Support.svelte';

  import Navbar from './components/Navbar.svelte';
  import 'material-icons/iconfont/material-icons.css';
  
  let page = 'home';

  function setPage(e) {
    const target = e.target.parentElement.classList.contains('navbar') ? e.target : e.target.parentElement;
    document.querySelector(`.navbar #${page}`).classList.remove('selected');
    page = target.id;
    target.classList.add('selected');
  }

  const navbarProps = { setPage };
</script>

<main>
  <Navbar {...navbarProps}/>

  {#if page === 'home'}
  <Home />
  {:else if page === 'rules'}
  <Rules />
  {:else if page === 'vote'}
  <Vote />
  {:else if page === 'staff'}
  <Staff />
  {:else if page === 'wiki'}
  <Wiki />
  {:else if page === 'support'}
  <Support />
  {/if}

</main>
