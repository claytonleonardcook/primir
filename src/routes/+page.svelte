<script lang="ts">
  import Button from "../components/atoms/Button.svelte";

		  let counter = 0;
</script>

<h1>Clicker: {counter}</h1>
<Button on:click={() => counter++}>Click Me!</Button>

<style>
		  
</style>
