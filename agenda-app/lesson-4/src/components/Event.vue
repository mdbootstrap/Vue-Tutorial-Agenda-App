<template>
  <div>
    <h3>{{time}} - {{title}}</h3>
    <p>{{location}}</p>
    <p>{{description}}</p>
  </div>
</template>

<script>
export default {
  name: "Event",
    props: {
    time: {
      type: String
    },
    title: {
      type: String
    },
    location: {
      type: String
    },
    description: {
      type: String
    }
  },
};
</script>

<style scoped>
</style>
