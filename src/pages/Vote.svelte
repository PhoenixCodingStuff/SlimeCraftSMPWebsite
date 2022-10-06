<script>
    const voteUris = [
        'https://minecraft-mp.com/server/309322/vote/',
        'https://minecraft-server.net/vote/SlimeCraftSMP/',
        'https://minecraftservers.org/server/641185',
        'https://topmcservers.com/server/2127/vote',
        'https://servers-minecraft.net/server-slimecraftsmp.21927'
    ];
</script>

<main>
    <button class="offset inverted" on:click="{e => voteUris.forEach(uri => window.open(uri))}">
        Vote on All!
    </button>
    <br/>
    <button class="offset" on:click="{e => window.open(voteUris[0])}">
        Vote on minecraft-mp.com
    </button>
    <br/>
    <button class="offset" on:click="{e => window.open(voteUris[1])}">
        Vote on minecraft-server.net
    </button>
    <br/>
    <button class="offset" on:click="{e => window.open(voteUris[2])}">
        Vote on minecraftservers.org
    </button>
    <br/>
    <button class="offset" on:click="{e => window.open(voteUris[3])}">
        Vote on topmcservers.com
    </button>
    <br/>
    <button class="offset" on:click="{e => window.open(voteUris[4])}">
        Vote on servers-minecraft.net
    </button>
</main>
