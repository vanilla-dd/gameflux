<script lang="ts">
	import { Button } from './ui/button';
</script>

<nav class="flex items-center justify-between px-4 py-2 shadow-md">
	<div class="">logo</div>
	<div>
		<a href="/"><Button variant="link">Home</Button> </a>
		<a href="/events"><Button variant="link">Events</Button> </a>
		<a href="/rules"><Button variant="link">Rules</Button> </a>
		<Button variant="outline">Login</Button>
	</div>
</nav>
