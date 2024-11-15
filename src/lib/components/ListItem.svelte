<script>
	let { icon, title, index, focusAction, correctAnswer, incorrectAnswer } = $props();
	let ABC = 'ABCDEFGHIJKLMNOPYRSTUVWXYZ';
</script>

<button class="alert flex focus:outline focus:outline-primary" onfocus={focusAction}>
	{#if icon}
		<img src={icon} alt={title + '-Icon'} />
	{:else}
		<span>{ABC[index]}</span>
	{/if}
	<span>{title}</span>
</button>
