<template>
  <div id="app">
    <nav-menu @selectMenu="onChangeMenu"></nav-menu>
    <results :resultData="results" v-show="selected == 1"></results>
  </div>
</template>

<script>
import { results } from './data/mock';
import { NavMenu, Results } from './components';
// import { bus } from './utils/event';
export default {
  data () {
    return {
      results,
      selected: 1,
    }
  },
  components: {
    NavMenu,
    Results,
  },
  methods: {
    onChangeMenu (data) {
      console.log(data, this.selected);
      this.selected = data;
      // this.$set('selected', data); // error
    },
  },
}
</script>

<style>
body {
  font-family: Helvetica, sans-serif;
  margin: 0 auto;
  width: 100%;
  height: 100%;
}
</style>
