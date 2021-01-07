<script>
	import Card from './Posts/Card.svelte';
	import Header from './Design/Header.svelte';
	const color = "warning"
	const post = [
		{
			id:'1',
			title: 'Working with Svelte',
			description:'Svelte In the Morning',
			imagen: 'https://cdn.pixabay.com/photo/2020/12/29/10/07/coast-5870088_1280.jpg'
		},
		{
			id:'2',
			title: 'Working with Svelte',
			description:'Svelte In the Affternoon',
			imagen: 'https://cdn.pixabay.com/photo/2021/01/01/14/07/chapel-5878656_1280.jpg'
		},
		{
			id:'3',
			title: 'Working with Svelte',
			description:'Svelte at nigth',
			imagen: 'https://cdn.pixabay.com/photo/2020/12/28/18/32/mountains-5868127_1280.jpg'
		}
	]
</script>

<Header title="Components" {color}/>
<Header title="Mi Second Navbar" color="info"/>

<div class="container">
	{#each post as item}
		<Card>
			title = {item.title}
			description = {item.description}
			imagen = {item.imagen}
		</Card>

	{/each}
</div>