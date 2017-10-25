<template>
  <div class='container'>
    <div class='row'>
      <div class='col-xs-12'>
        <button @click='selectedComponent = "appQoute"'>Quote</button>
        <button @click='selectedComponent = "appAuthor"'>Author</button>
        <button @click='selectedComponent = "appNew"'>New</button>
        <p> {{ selectedComponent }}</p>
        <hr>
        <keep-alive>
          <component :is='selectedComponent'>
            <p>Default Content</p>
          </component>
        </keep-alive>
      </div>
    </div>
  </div>
</template>

<script>
  import Qoute from './components/Qoute.vue';
  import Author from './components/Author.vue';
  import New from './components/New.vue';

  export default {
    data: function() {
      return {
        quoteTitle: "The Quote",
        selectedComponent: 'appQoute'
      }
    },
    components: {
      appQoute: Qoute,
      appAuthor: Author,
      appNew: New
    }
  }
</script>

<style lang="scss">
</style>
