<script>
	// export let name;
	import  Navbar  from "./pages/Navbar.svelte";
	import  SectionA  from "./pages/Section-A.svelte";
	import  SectionB  from "./pages/Section-B.svelte";
	import  SectionC  from "./pages/Section-C.svelte";
	import  SectionD  from "./pages/Section-D.svelte";
</script>

<svelte:head>
	<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.6.1/dist/css/bootstrap.min.css" integrity="sha384-zCbKRCUGaJDkqS1kPbPd7TveP5iyJE0EjAuZQTgFLD2ylzuqKfdKlfG/eSrtxUkn" crossorigin="anonymous">

</svelte:head>

<style>
	main{
		font-family: 'Basic', sans-serif;
	}
	

</style>

<main>
	<Navbar/>
	<SectionA/>
	<SectionB/>
	<SectionC/>
	<SectionD/>


	
	<script src="https://cdn.jsdelivr.net/npm/jquery@3.5.1/dist/jquery.slim.min.js" integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj" crossorigin="anonymous"></script>
	<script src="https://cdn.jsdelivr.net/npm/bootstrap@4.6.1/dist/js/bootstrap.bundle.min.js" integrity="sha384-fQybjgWLrvvRgtW6bFlB7jaZrFsaBXjsOMm/tB9LTS58ONXgqbR9W8oWht/amnpF" crossorigin="anonymous"></script>
</main>
