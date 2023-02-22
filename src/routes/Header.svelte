<script>
	import { page } from '$app/stores'

	import Theme from '../lib/components/theme.svelte'
</script>

<header class="container">
	<nav>
		<ul>
			<li
				aria-current={$page.url.pathname === '/'
					? 'page'
					: undefined}
			>
				<a href="/">Home</a>
			</li>
			<li
				aria-current={$page.url.pathname === '/about'
					? 'page'
					: undefined}
			>
				<a href="/about">About</a>
			</li>
		</ul>
	</nav>
	<Theme />
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
	}

	nav {
		display: flex;
		justify-content: center;
		--background: rgba(255, 255, 255, 0.7);
	}
</style>
