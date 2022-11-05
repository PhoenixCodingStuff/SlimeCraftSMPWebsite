<script>
    import DiscordLogo from "../assets/discord.svg";
    export let navigateTo;

    const discordInvite = 'https://discord.gg/DZVDucC4jG';
    const wikiInvite = 'https://slimecraftsmpwiki.gitbook.io/slimecraftsmp/';
</script>

<nav class='navbar'>
    <span></span>
    <span id='home' tabindex="0" on:click={() => navigateTo('home')} on:keypress={() => navigateTo('home')}>
        <span class="material-icons">home</span>
        Home
    </span>
    <span tabindex="0" on:click={() => window.open(discordInvite)} on:keypress={() => window.open(discordInvite)}>
        <img src={DiscordLogo} alt="Discord logo"/>
        Discord
        <span class="material-icons">open_in_new</span>
    </span>
    <span id='rules' tabindex="0" on:click={() => navigateTo('rules')} on:keypress={() => navigateTo('rules')}>
        <span class="material-icons">menu_book</span>
        Rules
    </span>
    <span id='vote' tabindex="0" on:click={() => navigateTo('vote')} on:keypress={() => navigateTo('vote')}>
        <span class="material-icons">check_box</span>
        Vote
    </span>
    <span id='staff' tabindex="0" on:click={() => navigateTo('staff')} on:keypress={() => navigateTo('staff')}>
        <span class="material-icons">manage_accounts</span>
        Staff
    </span>
    <span tabindex="0" on:click={() => window.open(wikiInvite)} on:keypress={() => window.open(wikiInvite)}>
        <span class="material-icons-outlined">info</span>
        Wiki
        <span class="material-icons">open_in_new</span>
    </span>
    <span id='support' tabindex="0" on:click={() => navigateTo('support')} on:keypress={() => navigateTo('support')}>
        <span class="material-icons">settings</span>
        Support
    </span>
    <span id='gallery' tabindex="0" on:click={() => navigateTo('gallery')} on:keypress={() => navigateTo('gallery')}>
        <span class="material-icons">photo_library</span>
        Gallery
    </span>
    <span></span>
</nav>

<style>
    .navbar {
        font-family: 'Silkscreen', cursive;
        background-color: #007a1a;
        height: 80px;
        color: #17dd61;
        display: flex;
        justify-content: space-around;
        align-items: center;
    }

    .navbar > span {
        cursor: pointer;
        padding: 16px;
        font-size: 20px;
        display: flex;
        align-items: center;
    }

    span > img, span > span {
        width: 24px;
        height: 24px;
        margin-right: 8px;
    }
</style>
