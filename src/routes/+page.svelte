<script>
	let imageVisible = false
	let msgVisible = false
	let message = ''
	let image

	function showMessage() {
		if (msgVisible) {
			message = ''
			msgVisible = false
		} else {
			message = 'Iloveyou'
			msgVisible = true
		}
		console.log(message)
	}

	function toggleImage() {
		image = document.getElementById('image')
		image.src = '/love.png'
		if (imageVisible) {
			image.style.display = 'none'
			imageVisible = false
		} else {
			image.style.display = 'block'
			imageVisible = true
		}
	}
</script>

<h1>This is {message}</h1>

<button on:click={showMessage}
	>Click me! I have surprise</button
>
<img id="image" alt="" />
<button on:click={toggleImage}>Show Image</button>

<style>
	h1 {
		color: goldenrod;
		font-family: 'Comic Sans MS', cursive;
		font-size: 2em;
	}

	button {
		border: 1px solid black;
		padding: 2px;
		border-radius: 5px;
	}
</style>
