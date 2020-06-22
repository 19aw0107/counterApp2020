<template>
  <div id="count">
    <p>{{ $store.state.count }}</p>
    <button @click="increment"><p>+</p></button>
    <button @click="decriment"><p>-</p></button>
  </div>
</template>
<script>
export default {
  methods:{
    increment(){
      this.$store.commit('increment')
    },
    decriment(){
      this.$store.commit('decriment')
    }
  },
  computed:{
    count(){
      return this.$store.getters.count
    }
  }
  /*computed:{
    count(){
      return this.$store.state.count
    }
  }*/
}
</script>
