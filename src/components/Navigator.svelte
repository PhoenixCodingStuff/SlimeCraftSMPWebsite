<script>
    import { Route, useLocation, useNavigate } from "svelte-navigator";
    import Home from '../pages/Home.svelte';
    import Rules from '../pages/Rules.svelte';
    import Vote from '../pages/Vote.svelte';
    import Staff from '../pages/Staff.svelte';
    import Support from '../pages/Support.svelte';
    import Gallery from '../pages/Gallery.svelte';
    import Navbar from './Navbar.svelte';

    const location = useLocation();
    const navigate = useNavigate();

    window.onload = () => {
        try { document.querySelector(`#${$location.pathname.slice(1)}`).classList.add('selected'); }
        catch (e) { document.querySelector('#home').classList.add('selected'); }
    }

    const navigateTo = (page) => {
        document.querySelector('.selected').classList.remove('selected');
        document.querySelector(`#${page}`).classList.add('selected');
        navigate(`/${page}`);
        window.scrollTo({ top: 0, behavior: 'smooth' });
    }
</script>

<Navbar navigateTo={navigateTo} />

<Route> <Home navigateTo={navigateTo} /> </Route>
<Route path="rules"> <Rules /> </Route>
<Route path="vote"> <Vote /> </Route>
<Route path="staff"> <Staff /> </Route>
<Route path="support"> <Support navigateTo={navigateTo} /> </Route>
<Route path="gallery"> <Gallery /> </Route>
