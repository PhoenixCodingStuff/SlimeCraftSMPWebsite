<script>
  import Home from './pages/Home.svelte';
  import Rules from './pages/Rules.svelte';
  import Vote from './pages/Vote.svelte';
  import Staff from './pages/Staff.svelte';
  import Support from './pages/Support.svelte';

  import Navbar from './components/Navbar.svelte';
  import 'material-icons/iconfont/material-icons.css';
  
  let page = 'home';

  function setPage(e) {
    const target = e.target.classList.contains('material-icons') ? e.target.parentElement : e.target;
    document.querySelector(`.navbar #${page}`).classList.remove('selected');
    page = target.id;
    target.classList.add('selected');
    window.scrollTo({ top: 0, behavior: 'smooth' });
  }

  const navbarProps = { setPage };
  const supportProps = { setPage };
</script>

<main class="expand">
  <Navbar {...navbarProps}/>

  {#if page === 'home'}
  <Home />
  {:else if page === 'rules'}
  <Rules />
  {:else if page === 'vote'}
  <Vote />
  {:else if page === 'staff'}
  <Staff />
  {:else if page === 'support'}
  <Support {...supportProps}/>
  {/if}

</main>

<style>
  .expand {
    flex-grow: 1;
  }
</style>
