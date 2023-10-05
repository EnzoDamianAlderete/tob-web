<script>
	  import Navbar from "$lib/components/Navbar.svelte";
import "../app.postcss";
</script>

<div class="min-h-screen">
	<Navbar />
	<main class="w-full flex flex-col">
		<slot />
	</main>
</div>

