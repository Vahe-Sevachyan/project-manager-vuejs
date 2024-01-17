<template>
  <div v-bind:key="task.id" v-for="task in SetTasks">
    <h3>{{ task.text }}</h3>
  </div>
</template>
<script>
export default {
  name: "SetTasks",
  props: {
    tasks: Array,
  },
};
</script>
