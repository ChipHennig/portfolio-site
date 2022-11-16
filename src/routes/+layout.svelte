
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
		color: white;
		font-size: 2em;
		background-image: url('/Malojapass_Böhringer_2018-min.jpg');
		background-attachment: fixed;
		background-size: cover;
	}
</style>
