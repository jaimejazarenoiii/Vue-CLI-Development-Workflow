<template>
  <div>
    <div class='title'>
      <slot name='title'></slot>
    </div>
    <div>
      <slot name='content'></slot>
    </div>
  </div>
</template>

<script>
  export default{
    props: {
      qoute: {
      }
    }
  }
</script>

<style scoped>
  div{
    border: 1px solid #ccc;
    box-shadow: 1px 1px 2px black;
    padding: 30px;
    margin: 30px auto;
    text-align: center;
  }
</style>
