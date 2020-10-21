<script>
  import {createEventDispatcher} from "svelte";

  let dispatch = createEventDispatcher();

  let backDrop;

  const handleBackdrop = () => {
    const backdrop = backDrop;
    dispatch('backdrop', backdrop);
  }

</script>

<style>
  .backdrop {
    position: fixed;
    display: none;
    top: 0;
    left: 0;
    z-index: 100;
    width: 100vw;
    height: 100vh;
    background: rgba(0, 0, 0, 0.5);
  }
</style>

<div
bind:this={backDrop}
on:click={handleBackdrop}
class="backdrop" />
