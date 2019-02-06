<template>
  <div class="app">
    <h2>I am App (main component)</h2>
    <HelloWorld/>
  </div>
</template>

<script>
import HelloWorld from "@/components/HelloWorld";

export default {
  name: "App",
  components: {
    HelloWorld
  }
};
</script>

<style>
.app {
  margin: 0 auto;
  font-family: sans-serif;
  background-color: #ccf7e2;
  padding: 10px;
  border-radius: 5px;
  max-width: 500px;
}
</style>