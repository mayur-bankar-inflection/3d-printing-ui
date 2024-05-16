<script>
	import '../app.css';
	// import '../app.css';
	import Navbar from '$lib/Components/Navbar.svelte';
	import Footer from '$lib/Components/Footer.svelte';
</script>

<Navbar></Navbar>
<slot></slot>
<Footer/>
