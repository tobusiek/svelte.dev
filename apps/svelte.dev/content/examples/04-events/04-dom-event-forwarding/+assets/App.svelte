<script>
	import CustomButton from './CustomButton.svelte';

	function handleClick() {
		alert('clicked');
	}
</script>

<CustomButton onclick={handleClick} />
