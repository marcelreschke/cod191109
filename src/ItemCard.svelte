<style>
@import url('https://fonts.googleapis.com/css?family=Open+Sans&display=swap');
h1,p {font-family:Open Sans;}
</style>

<script>
    export let item;
</script>

<section class="ItemCard">
    <img width="200px" src="{item.Bild}" alt="Bild von {item.Name}">
    <section> 
        <b style="font-size:25px; color:navy">Student {item.ID}</b>
        <ul>
        <li style="font-size:20px">Name: {item.Name}</li>
        <li style="font-size:20px">Geburtsdatum: {item.Geburtsdatum}</li>
        <li style="font-size:20px">Geschlecht: {item.Geschlecht}</li>
        <li style="font-size:20px">Studiengang: {item.Studiengang}</li>
        <li style="font-size:20px">Matrikelnummer: {item.Martrikelnummer}</li>
        </ul>
    </section>
</section>
