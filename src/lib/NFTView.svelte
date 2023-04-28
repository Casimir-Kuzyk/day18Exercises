<script lang="ts">
    import { onMount } from 'svelte';

    type NFT = {
        name: String,
        description: String
    }

    let nfts: NFT[] = [];

    onMount(() => {
        const interval = setInterval(() => {
            nfts.push({name: 'New NFT', description: 'this is an NFT'});
            nfts = [...nfts];
        }, 5000);
        return () => clearInterval(interval);
    });
</script>

{#each nfts as nft}
    <div>
        <h2>{nft.name}</h2>
        <p>{nft.description}</p>
    </div>
{/each}