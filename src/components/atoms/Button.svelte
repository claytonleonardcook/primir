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
					 scale: 1;
		  }

		  button:focus {
					 -webkit-animation: click 0.5s;
					 animation: click 0.5s;
		  }

		  button:active {
					 -webkit-animation: none;
					 animation: none;
		  }

		  @keyframes click {
					16% {
					 scale: 1.1;
					}
					50% {
					 scale: 1;
					}
		  }
</style>
