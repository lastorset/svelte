<script>
	// `value` is updated whenever the prop value changes...
	export let value;

	// ...but `color` is fixed upon initialisation
	const color = value;
</script>

<p style="background-color: {color}">{color} / {value}</p>