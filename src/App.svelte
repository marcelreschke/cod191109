<script>
    import Nested from './Nested.svelte';
    import Button from './Button.svelte';
    import Header from './Header.svelte';
    import ItemDetail from './ItemDetail.svelte';
    import ItemList from './ItemList.svelte';
    import Modal from './Modal.svelte';
    import './studentendaten.json';
   
   function handleMessage(event) {
        alert(event.detail.text);
    }
</script>

<style>

</style>
<Header title="Studentendaten" subtitle="Deine Studentendaten auf einen Blick"/>
<h1><center>Time for a project!</center></h1>
<Nested/>
<Button ButtonText="Start" AltButtonText="Finish" on:message={handleMessage}/>