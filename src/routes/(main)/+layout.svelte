<script lang="ts">
import type { Snippet } from "svelte";

const {
	children,
}: {
	children: Snippet<[]>;
} = $props();
</script>

<div class="wrap">
	<div class="navBar">
	    <div class='navBarInner'>
			<h2>Games!</h2>
		</div>
	</div>
	<div class="content">
		{@render children?.()}
	</div>
</div>

<style lang="scss">
    .wrap {
        display: flex;
        flex-direction: column;
    }
</style>
