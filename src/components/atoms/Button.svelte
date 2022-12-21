<script lang="ts">

</script>

<button {...$$restProps} on:click>
		  <slot />
</button>

<style>
		  button {
					 all: unset;
					 height: 1em;
					 width: fit-content;
					 padding: 0.5rem;
					 border: solid #000 1px;
					 border-radius: 0.5em;
					 background-color: #FFF;
					 color: #000;
					 transition-duration: 0.5s;
					 cursor: pointer;
		  }

		  button:hover {
					 background-color: #000;
					 color: #FFF;
		  }
</style>
