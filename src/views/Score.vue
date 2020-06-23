<template>
  <div class="score">
    <p>{{ $store.state.count }}</p>
    <!--<h1>This is an score page</h1>-->
  </div>
</template>
<script>
export default {
  computed:{
    count(){
      return this.$store.getters.count
    }
  }
}
</script>