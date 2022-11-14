
<div>
	<nav>
		<a href="/">Christian Hennig</a>
		<a href="/history">About</a>
		<a href="/credits">Contact</a>
	</nav>
	<slot />
</div>

<style>
	:global(a) {
		color: crimson;
	}
	:global(body) {
		height: 100vh;
		color: white;
		font-size: 2em;
		background-image: url('/fisheye_night.jpg');
		background-attachment: fixed;
		background-size: cover;
	}
</style>
