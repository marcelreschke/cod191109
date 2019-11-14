<script>
    import ItemCard from './ItemCard.svelte'

    export let items = [];
</script>

<style>

@import url('https://fonts.googleapis.com/css?family=Dosis&display=swap');
h1,p {font-family:Dosis;}

h1 {
    font-weight: 700;
    line-height: 1.5;
}

p {
    line-height: 0.8;

}

.student { 
    background-color: lightskyblue;
    width: 400px;
    padding: 10px;
    border: solid 4px #000000;
    margin:10px;


}

.liste { 
    background-color: rgb(68, 141, 215);
    padding: 10px;
    border: solid 4px #000000;
    margin:10px;

}
</style>

<section class="liste">
    {#each items as item, i}
    <section class="student">
        <ItemCard {item}/>
    </section>
    {/each}
</section>