<template>
	<p>Amount of ToDos: {{todos.length}}</p>
</template>

<script>

export default ({
	props:{
		todos:{
			type: [Object, Array]
		}
	}
})
</script>
