<script>
    import DiscordLogo from "../assets/discord.svg";
    export let setPage;

    const discordInvite = 'https://discord.gg/EtW8FCeGV7';
    const wikiInvite = 'https://slimecraftsmpwiki.gitbook.io/slimecraftsmp/'
</script>

<div class='navbar'>
    <span id='home' class="selected" on:click={setPage}>
        <span class="material-icons">home</span>
        Home
    </span>
    <span id='invite' on:click="{e => window.open(discordInvite)}">
        <img src={DiscordLogo} alt="Discord logo"/>
        Discord
        <span class="material-icons">open_in_new</span>
    </span>
    <span id='rules' on:click={setPage}>
        <span class="material-icons">menu_book</span>
        Rules
    </span>
    <span id='vote' on:click={setPage}>
        <span class="material-icons">check_box</span>
        Vote
    </span>
    <span id='staff' on:click={setPage}>
        <span class="material-icons">manage_accounts</span>
        Staff
    </span>
    <span id='wiki' on:click="{e => window.open(wikiInvite)}">
        <span class="material-icons-outlined">info</span>
        Wiki
        <span class="material-icons">open_in_new</span>
    </span>
    <span id='support' on:click={setPage}>
        <span class="material-icons">settings</span>
        Support
    </span>
</div>

<style>
    .navbar {
        font-family: 'Silkscreen', cursive;
        background-color: #007a1a;
        margin: 0;
        padding-left: 128px;
        padding-right: 128px;
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

    .selected {
        color: #aeffcd;
    }
</style>
