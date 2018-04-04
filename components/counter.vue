<template>
<div>
    Value : {{counter}}
    <button @click="$store.commit('increment')">+</button>
    <button @click="$store.commit('decrement')">-</button>
</div>
</template>

<script>
import { mapState } from 'vuex'

export default {
  computed: {
    ...mapState({
        counter: state => state.counter,
    })
  }
};
</script>

<style scoped>

</style>
