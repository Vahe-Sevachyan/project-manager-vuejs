<template>
  <div v-bind:key="task.id" v-for="task in SetTasks">
    <h3>{{ task.text }}</h3>
    <TasksList :task="task" />
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
<style>
.task {
  background: 5px;
  margin: 5px;
  padding: 10px 20px;
  cursor: pointer;
}
.task.runner {
  border-left: 5px solid green;
}
.task h3 {
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
