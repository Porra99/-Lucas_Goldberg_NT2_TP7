<template>

<div id="game">
     <ul  v-for="(color, index) in $store.state.colors" :key="color.id">
         <ColorItems v-if="hasWon"  :color="$store.state.pickedColor" :i="index" />
         <ColorItems v-else  :color="$store.state.colors[index]" :i="index" />
    </ul>   
</div>

</template>

<script lang="js">
  import ColorItems from './ColorItems.vue'
  export default  {
    name: 'Game',
    components:{ 
        ColorItems
    },
    mounted () {

    },
    data () {
      return {
      }
    },
    methods: {
    },
    computed: {
    }
}

</script>

<style scoped lang="css">
#game {
	margin: 20px auto;
	max-width: 600px;
}
</style>