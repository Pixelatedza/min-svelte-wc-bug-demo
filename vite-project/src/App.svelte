<svelte:options tag='custom-element'/>

<script>
  import {someStore} from './store.js';
  $: console.log($someStore);
</script>

<button on:click={() => someStore.update(n => n + 1)}>Change store value</button>
<p>A minimal example of duplicate elements</p>
