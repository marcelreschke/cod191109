<script>
    import Nested from './Nested.svelte';
    import Button from './Button.svelte';
   
   function handleMessage(event) {
        alert(event.detail.text);
    }
</script>

<style>

</style>

<h1><center>Time for a project!</center></h1>
<Nested/>
<Button ButtonText="Start" AltButtonText="Finish" on:message={handleMessage}/>