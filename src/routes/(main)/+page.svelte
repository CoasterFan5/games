<script>
import GameCard from "./GameCard.svelte";
</script>
<div class="gameSection">
	<h2>Alphas</h2>
	<p>More than just playable, games that are semi-fleshed out.</p>
	<a href="https://heardle.coasterfan5.com" target="_blank"
		>Heardle Unlimited</a
	>
</div>
<div class="gameSection">
	<h2>Demos</h2>
	<p>
		Playable but not done. Just a concept. This is where most of my games fall.
	</p>
	<a href="https://glimpse.coasterfan5.com" target="_blank">Black Box</a>
	<a href="https://tacos.coasterfan5.com" target="_blank">Lucky Tacos</a>
	<a href="https://lost-drone.coasterfan5.com" target="_blank"
		>Lost Drone Protocol</a
	>
</div>

<style lang="scss">
    h2 {
        margin: 0;
    }
    p {
        margin: 0;
    }

    .gameSection {
        display: flex;
        flex-direction: column;

        a {
            color: var(--color);
            &:hover {
                color: var(--accent);
            }
        }
    }
</style>
