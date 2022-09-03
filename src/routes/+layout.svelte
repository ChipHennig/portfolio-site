<div id="back">
	<nav>
		<a href="/">Home</a>
		<a href="/history">About</a>
		<a href="/credits">Contact</a>
	</nav>
	<img src={'/denmark.jpg'} alt="Northern lights" />
	<slot />
</div>

<style>
	img {
		width: 100%;
		height: 30vh;
		object-fit: cover;
	}
	:global(a) {
		color: white;
	}
	:global(body) {
		height: 100vh;
		color: white;
		font-size: 2em;
		background-color: tan;
	}
</style>
