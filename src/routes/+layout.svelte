
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
		color: maroon;
	}
	:global(body) {
		height: 100vh;
		color: black;
		font-size: 2em;
		background-image: url('/swiss_mountains-min.jpg');
		background-attachment: fixed;
		background-size: cover;
	}
</style>
