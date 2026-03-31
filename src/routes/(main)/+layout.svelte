<script lang="ts">
import { resolve } from "$app/paths";
import type { Snippet } from "svelte";

const {
	children,
}: {
	children: Snippet<[]>;
} = $props();
</script>

<div class="wrap">
	<div class="navBar">
		<div class="navBarInner">
			<div class="left">
				<h2><a href="/" class="homePage"> games.coasterfan5.com </a></h2>
			</div>
			<div class="right">
				<a class="link" href={resolve("/(main)/about")}>about</a>
			</div>
		</div>
	</div>
	<div class="content">{@render children?.()}</div>
</div>

<style lang="scss">
    .wrap {
        display: flex;
        flex-direction: column;
    }

    .navBar {
        display: flex;
        align-items: center;
        justify-content: center;
        background: var(--background-alt);
        border-bottom: 1px solid var(--border);
    }

    .navBarInner {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 1rem;
        width: 100%;
    }

    h2 {
        margin: 0px;
        font-size: 1.2rem;
        font-weight: 500;
    }

    .homePage {
        color: var(--color);
        text-decoration: none;
    }

    .link {
        color: var(--color);
        text-decoration: none;
        &:hover {
            color: var(--accent);
        }
    }

    .content {
        width: 100%;
        padding: 1rem;
    }
</style>
