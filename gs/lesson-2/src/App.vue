<template>
  <div class="app">
    <h1>This is your first component in Vue</h1>
    <h3>{{ message }}</h3>
    <ul>
      <li>{{ number + 1 }}</li>
      <li>Value of ok var is: + {{ ok ? 'true' : 'false' }}</li>
      <li>{{ message.split('').reverse().join('') }}</li>
    </ul>
    <span v-if="visible">Now you see me</span>
    <ol>
      <li v-for="todo in todos">{{ todo.text }}</li>
    </ol>
    <p>Original message: "{{ message }}"</p>
    <p>Computed reversed message: "{{ reversedMessage }}"</p>
  </div>
</template>

<script>
export default {
  name: "App",
  data: () => ({
    message: "Powered by MDB!",
    number: 5,
    ok: true,
    visible: true,
    todos: [
      { text: "Learn JavaScript" },
      { text: "Learn Vue" },
      { text: "Build something awesome" }
    ]
  }),
  computed: {
    // a computed getter
    reversedMessage: function() {
      // `this` points to the vm instance
      return this.message
        .split("")
        .reverse()
        .join("");
    }
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