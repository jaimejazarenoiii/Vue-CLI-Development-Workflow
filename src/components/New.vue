<template>
  <div>
    <h1>New Quote</h1>
    <button @click='counter++'>Increase!</button>
    <p>{{ counter }}</p>
  </div>
</template>

<script>
  export default{
    data: function() {
      return {
        counter: 0
      }
    }
  }
</script>

<style>

</style>
