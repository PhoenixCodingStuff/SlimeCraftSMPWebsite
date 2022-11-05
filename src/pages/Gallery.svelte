<script>
    import ServerBanner from "../assets/server-banner.png";
    import ServerSpawnNight from "../assets/server-spawn-night.png";
    import ServerCustomVillage from "../assets/server-custom-village.png";
    import ServerSkyIsland from "../assets/server-sky-island.png";
    import ServerVolcano from "../assets/server-volcano.png";

    const imgData = [
        { "id": 1, "params": { "src": ServerBanner, "alt": "SlimeCraftSMP Spawn" } },
        { "id": 2, "params": { "src": ServerSpawnNight, "alt": "SlimeCraftSMP Spawn at Night" } },
        { "id": 3, "params": { "src": ServerCustomVillage, "alt": "SlimeCraftSMP Custom Village" } },
        { "id": 4, "params": { "src": ServerSkyIsland, "alt": "SlimeCraftSMP Sky Island" } },
        { "id": 5, "params": { "src": ServerVolcano, "alt": "SlimeCraftSMP Volcano" } }
        ];
</script>

<main>
    {#each imgData as data (data.id)}
        <img { ...data.params } />
    {/each}
</main>

<style>
    main {
        display: flex;
        flex-direction: column-reverse;
        align-items: center;
        padding-top: 64px;
    }
    img {
        aspect-ratio: initial;
        width: 45rem;
        margin-bottom: 64px;
    }
</style>
