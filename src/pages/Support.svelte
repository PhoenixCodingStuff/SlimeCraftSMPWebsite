<script>
    import McGrassBlock from "../assets/mc-grass-block.svg";
    export let setPage;

    const guidelinesUri = 'https://discord.com/channels/923817461550297108/923817461877456905/972042285082624010';
    const staffTicketUri = 'https://discord.com/channels/923817461550297108/923817461877456905/999279418017054801';
    const donateTicketUri = 'https://discord.com/channels/923817461550297108/923817461877456905/999279857865334845';
    const bugTicketUri = 'https://discord.com/channels/923817461550297108/923817461877456905/999280290952388608';
    const hackerTicketUri = 'https://discord.com/channels/923817461550297108/923817461877456905/999280605374189598';
    const questionTicketUri = 'https://discord.com/channels/923817461550297108/923817461877456905/999280893795508334';
    const discordInvite = 'https://discord.gg/d4GJ3EbhUR';
</script>

<main class="container">
    <img class="mc-grass-block" src={McGrassBlock} alt="Minecraft grass block"/>
    <iframe title="List of online Discord server members" src="https://discord.com/widget?id=923817461550297108&theme=dark" width="350" height="500" allowtransparency="true" frameborder="0" sandbox="allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts"></iframe>
    <br/>

    <h1>Support Guidelines</h1>
        <p>
            Need help? You can create a ticket on our <a href={discordInvite} target="_blank">discord server</a>!
            There are some <a href={guidelinesUri}>guidelines</a> though.
        </p>
    <br/>
    <h2>Help! A Staff is abusing his/her powers!</h2>
        <p>
            Found a staff abusing his/her powers? Have an issue with how one handed a situation?
            <br/>You can <a href={staffTicketUri} target="_blank">create a ticket</a>!
            <br/>Handled by an Admin+ , if you have an issue with an Admin+ please DM PhoenixPlayz#1880.
        </p>
    <br/>
    <h2>I donated but did not get my rank! You scammer!</h2>
        <p>
            Did you donate but did not get your perks? Did you not recieve a rank/item you won from giveaway?
            <br/>You can <a href={donateTicketUri} target="_blank">create a ticket</a>!
            <br/>Do not worry! It happens sometimes due to unavoidable situations. Your rank/items will be given!
        </p>
    <br/>
    <h2>I found a game-breaking bug! This stuff does not work!</h2>
        <p>
            Found a dupe/exploit in game? Did you lose items due to a bug?
            <br/>You can <a href={bugTicketUri} target="_blank">create a ticket</a>!
            <br/>The bugs will be confirmed by staff and fixed by PhoenixPlayz#1880! Thank you for reporting and keeping the server safe!
        </p>
    <br/>
    <h2>This player is being toxic! Hacker! Help!</h2>
        <p>
            Found a hacker? Found a player breaking the server
            <span id='rules' on:click={setPage}>rules</span>?
            Your base was griefed?
            <br/>You can <a href={hackerTicketUri} target="_blank">create a ticket</a>!
            <br/>The player will be muted/banned. Grief will be rolled back. Your items will be refunded!
        </p>
    <br/>
    <h2>Oh I just have a question!</h2>
        <p>
            Have some questions about the server? Something that does not fit any other category?
            <br/>You can <a href={questionTicketUri} target="_blank">create a ticket</a>!
            <br/>Your questions will be answered within 24 hours
        </p>
    <br/><br/>
    <div class="blue-glow">
        Website by <a href="https://github.com/PhoenixCodingStuff" target="_blank">PhoenixCodingStuff</a>
        and <a href="https://mitulagrofficial.netlify.app/">mitulagrofficial</a>!
        <br/> Feel free to drop by with any concerns or if you like the website :)
    </div>
    <br/>
</main>

<style>
    iframe {
        display: block;
        margin: 0 auto;
    }

    .mc-grass-block {
        position: absolute;
    }

    #rules {
        color: #5865f2;
        cursor: pointer;
    }

    .blue-glow {
        color: #7777ff;
        text-shadow: 0 0 4px rgba(119, 119, 255, 170);
    }
</style>
