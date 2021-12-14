<template>
  <div id="app">
    <h1>Voici mon compteur</h1>
    <p>{{count}}</p>
    <Counter/>
  </div>
</template>

<script>
import index from './store/index.js'
import Counter from './components/Counter.vue'

export default {
  name: 'App',
  data(){
    return{
      index: index
    }
  },
  components:{
    Counter
  },
  computed:{
    count(){
      return index.state.count
    }
  }
}
</script>

<style>
</style>
