<template>
<div>
    <h1>Voici mes boutons</h1>
    <button @click='increment()'>+</button>
    <button @click='decrement()'>-</button>
</div>
</template>

<script>
import index from '../store/index.js'

export default {
    name: 'Counter',
    methods: {
        increment() {
            index.commit('increment')
        },
        decrement() {
            index.commit('decrement')
        },
    },
}
</script>

<style>

</style>
