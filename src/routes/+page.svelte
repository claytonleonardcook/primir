<script lang="ts">
  import Button from "../components/atoms/Button.svelte";

		  let counter = 0;
</script>

<h1>Count: {counter}</h1>
<Button on:click={() => counter++}>Click Me!</Button>
<br />
<Button on:click={() => {
		  if (!("Notification" in window)) {
					 alert("This browser doesn't support notifications!");
					 return;
		  }

		  if(Notification.permission === "denied") {
					 Notification.requestPermission().then((permission) => {
								if(permission === "granted") {
										  const notification = new Notification("Hello World!");
								}
					 });
					 return;
		  }
		  
		  const notification = new Notification("Hello World!");
}}>Send Notification in 10 Seconds</Button>

<style>
		  
</style>
