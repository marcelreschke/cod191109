<script>

    import { createEventDispatcher } from 'svelte';

    export let ButtonText;
    export let AltButtonText;

    let clicked =false;
    let active =false;

    const dispatch = createEventDispatcher();

    function expand() {
		dispatch('message', {
			text: 'Come back later!'
		});
	}

    function toggleButton () {
        active = !active;
        clicked = !clicked;
        if (clicked) expand();

    }

    
</script>

<style>

   button{
        background-color:transparent;
        border-radius:28px;
        border:1px solid #18ab29;
        display:inline-block;
        cursor:pointer;
	    color:#18ab29;
	    font-family:Arial, Helvetica, sans-serif;
	    font-size:17px;
	    padding:16px 31px;
	    text-decoration:none;
        position: relative;
        top: 50%;
        left: 50%;
	}
   button:hover{
       background-color: #18ab29;
       color: #ffffff
        
   }
   button:active{
       border: none;
       position: relative;
       outline: none;
   }
   .active{
        background-color: #18ab29;
        color: #ffffff;
   }
</style>

    {#if !clicked}
    <button class:active={active} on:click={toggleButton}>
        {ButtonText}
    </button>
    {:else}
    <button class:active={active} on:click={toggleButton}>
        {AltButtonText}
    </button>
    {/if}