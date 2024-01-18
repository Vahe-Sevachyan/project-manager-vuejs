<template>
  <div v-bind:key="task.id" v-for="task in SetTasks">
    <h3>{{ task.text }}</h3>
    <TasksList />
  </div>
</template>
<script>
import TasksList from "./TasksList";
export default {
  name: "SetTasks",
  props: {
    tasks: Array,
  },
  components: {
    TasksList,
  },
};
</script>
