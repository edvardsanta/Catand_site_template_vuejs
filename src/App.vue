<script setup>
import { ref } from 'vue'

const hiddenContent = ref(false);

function toggle() 
{
  hiddenContent.value = !hiddenContent.value;
}

</script>

<template>
	
	<header class="py-auto shadow-sm" id="port-header">
	<div v-show="hiddenContent" 
	class="text-black"
	> 
	<h1>Sobre mim</h1>
	<p class="text-muted">
								Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
							</p>	
	</div> 
        
	<div class="navbar mavbar-dark">
	<div class="container-fluid align-items-center">			
	
	<div id="imagem" class="py-3 col-xs-4 " align="center">		
	<h2>
							<a href="." class="text-muted">imagem</a>
						</h2>
	</div> <!--end of image-->

	<div id="logo" class="py-3 display-3 col-sm-4 d-none d-sm-block" style="width: 25%; height: 100%;"> 
		<a href="#" class="header-logo">Catand</a>
	</div>	<!-- end of logo -->

	<div id="button" class="py-3 icons-grid">
	  <b-button 
	class="mx-1 col"	 
	variant="outline-light" 
	@click="toggle"
	id="icon"
	>
        <b-icon-card-text
	size="5x"
	/>
	</b-button>
	</div> <!-- end of button -->
	</div> <!-- end of container-->
	</div>	<!-- end of navbar-->	     	
	
	</header>

	<main id="crown">
	<section class="py-5 text-center container">
        <div class="row py-lg-5">
	<div class="col-lg-6 col-md-8 mx-auto">
	<h1 class="fw-light">
		Exemplo
	</h1>
	<p class="lead text-muted">
				it is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. 
	</p>
	</div> <!-- end of col-->
	</div> <!-- end of row -->
	</section>
	</main>
</template>
<style scoped>
* 
{
  margin: 0;
  padding: 0;
}
/*ID*/
#port-header
{
  background-color: #DCDCDC;
}
#borda
{
  border: 1px solid red;
} 
#crown
{
  border-top: 3px solid gold;
  border-radius: 100%;
}
#logo
{
  margin: auto;                           width: 50%;
  padding: 10px;
  display: block;
}
#button                                 {
  width: 150px;
  height: 100px;
}
@media only screen and (max-width: 767px) 
{
	#button
	{
 		width: 15%;
		height: 20%;
	}	
}
#icon
{
  background-color: black;
  margin: 5px 0 0 15px;
  border: 1px dashed gold;
  border-radius: 10px;
}
#icon:hover
{
  background-color: white;
}

/*Class*/
.icons-grid 
{
  display: flex;
  flex-flow: row wrap;
  margin: -0;
}
.header-logo
{
  font-family: "Playfair Display", Georgia, "Times New Roman", sans-serif;
  text-decoration: none;
  color: black;
  font-size: 5rem;
  margin-right: 25px;
}
</style>
