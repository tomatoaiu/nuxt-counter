<template>
  <button @click="$store.commit('increment')">{{ counter }}</button>
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
