<template>
	<div id="header" :style="{ background: hasWon ? $store.state.pickedColor : 'blueviolet'  }">
		<h1>The Great <br>
			<span id="colorDisplay">{{ $store.state.pickedColor}} </span>
			<br>
			Guessing Game</h1>
	</div>
</template>

<script>
export default {
  name: 'JuegoColores',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#header {
	transition: all 0.3s;
	text-transform: uppercase;
	text-align: center;
	margin: 0;
	color: white;
}
#colorDisplay {
	font-size: 200%;
}

</style>
