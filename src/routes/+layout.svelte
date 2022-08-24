<nav>
	<a href="/">Home</a>
	<a href="/history">About</a>
	<a href="/credits">Settings</a>
</nav>

<slot />

<style>
	:not(iframe) {
        position: relative;
        z-index: 2;
		color: white;
		font-family: 'Comic Sans MS', cursive;
		font-size: 2em;
	}
</style>