<script>
    export let title;
    export let subtitle ;
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Cinzel&display=swap');

h1 {
font-family: 'Cinzel', serif;
position: absolute;
	top: 0px;
	left: 50%;
	width: 784px;
	height: 156px;

}



.topnav {
  background-color: #333;
  overflow: hidden;
  
}

.topnav a {


  float: left;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
    font-size: 17px;
    text-decoration: none;
 
}

.topnav a.active {
  background-color: #4CAF50;
  color: none;
  
}
.title {
    font-family: 'Cinzel', serif;
}

.subtitle{
    font-size: 0.8em;
    color: #f2f2f2;
    margin-left:8px;

}
</style>



<div class="topnav">
  <a href="/"><span class="title">{title}</span> <span class="subtitle">{subtitle}</span></a>
  
</div>



