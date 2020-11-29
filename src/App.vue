<template>
  <div id="app">
    <h1>Counter</h1>
    <counter :default-value="100" />
    <counter :default-value="75" />
    <counter />
  </div>
</template>

<script>
import Counter from "./components/Counter";

export default {
  name: "App",
  components: {
    Counter,
  },
};
</script>

<style>
</style>
