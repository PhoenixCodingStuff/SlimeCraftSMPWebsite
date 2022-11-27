<script>
    const voteUris = [
        'https://minecraft-mp.com/server/309322/vote', 
        'https://minecraftservers.org/server/643676', 
        'https://topmcservers.com/server/2127/vote', 
        'https://servers-minecraft.net/server-slimecraftsmp.21927', 
        'https://minecraft-server.net/vote/SlimeCraftSMP', 
        'https://topminecraftservers.org/vote/30726', 
        'https://minecraft-server-list.com/server/490560' 
    ];
</script>

<main class="container">
    <button class="offset inverted" on:click={e => voteUris.forEach(uri => window.open(uri))}>
        Vote on All!
    </button>
    <p class="caption">
        Make sure to enable popups for this website!
        <a href="https://support.google.com/chrome/answer/95472" target="_blank" rel="noreferrer">See How</a>.
    </p>
    <br/>
    <button class="offset" on:click={e => window.open(voteUris[0])}>
        Vote on minecraft-mp.com
    </button>
    <br/>
    <button class="offset" on:click={e => window.open(voteUris[1])}>
        Vote on minecraftservers.org
    </button>
    <br/>
    <button class="offset" on:click={e => window.open(voteUris[2])}>
        Vote on topmcservers.com
    </button>
    <br/>
    <button class="offset" on:click={e => window.open(voteUris[3])}>
        Vote on servers-minecraft.net
    </button>
    <br/>
    <button class="offset" on:click={e => window.open(voteUris[4])}>
        Vote on minecraft-server.net
    </button>
    <button class="offset" on:click={e => window.open(voteUris[5])}>
        Vote on topminecraftservers.org
    </button>
    <button class="offset" on:click={e => window.open(voteUris[6])}>
        Vote on minecraft-server-list.com
    </button>
</main>

<style>
    .caption {
        color: grey;
        text-align: center;
        margin: 0;
        margin-top: 16px;
        font-size: 0.8em;
    }

    button {
        --color: #1973bc;
        --hover: #19bc8b;
        display: block;
        color: var(--color);
        transition: 0.25s;
        background: none;
        border: 2px solid;
        font: inherit;
        line-height: 1;
        margin: auto;
        margin-top: 2em;
        padding: 1em 2em;
        box-shadow: 0.3em 0.3em 0 0 var(--color), inset 0.3em 0.3em 0 0 var(--color);
    }
    button:hover, button:focus {
        border-color: var(--hover);
        color: #fff;
        box-shadow: 0 0 0 0 var(--hover), inset 6em 3.5em 0 0 var(--hover);
    }

    .inverted {
        --color: #19bc8b;
        --hover: #1973bc;
    }
</style>
