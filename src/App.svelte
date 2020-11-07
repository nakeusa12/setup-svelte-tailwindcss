<script>
	import Tailwindcss from './Tailwindcss.svelte';
	let name = 'Nakeusa';
</script>

<style>
	/* main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	} */

	main {
		@apply w-full h-screen text-gray-500 bg-gray-200 py-12 px-48;
	}
	.card {
		@apply mx-auto flex items-center bg-indigo-500 rounded p-12;
	}
	.card-header {
		@apply w-2/5;
	}
	.card-header img {
		@apply object-cover object-center rounded;
	}
	.card-body {
		@apply w-3/5 flex flex-col pl-12;
	}

	h1 {
		@apply text-4xl mb-4 font-medium text-gray-200;
	}
	h3 {
		@apply text-xl mb-4 font-normal text-gray-200;
	}
	p {
		@apply text-gray-400 leading-relaxed;
	}
	p a.link {
		@apply text-gray-700;
	}
</style>

<main>
	<div class="card">
		<div class="card-header">
			<img
				alt="hero"
				src="https://images.pexels.com/photos/4954715/pexels-photo-4954715.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940" />
		</div>
		<div class="card-body">
			<h1>Welcome !</h1>
			<h3>My Name <b>"{name}"</b></h3>
			<p>
				This setup makes it easy for you so you don't have to bother setting it
				up again. you can check the source
				<a href="#" class="link">here</a>.
			</p>
		</div>
	</div>
</main>
