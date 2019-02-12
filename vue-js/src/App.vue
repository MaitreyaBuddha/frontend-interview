<template>
  <div id="app">
      <learn-mode :prompt="terms[0].word" />
  </div>
</template>

<script>
  import LearnMode from '@/components/LearnMode';
  import TERMS from './terms'
  
  export default {
    name: 'app',
    components: {
      LearnMode,
    },
    data() {
      return {
        terms: TERMS,
      };
    },
  };
</script>

<style>
body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
  margin: 0;
  padding: 0;
}
</style>
