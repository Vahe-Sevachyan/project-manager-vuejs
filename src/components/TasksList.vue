<template>
  <h3>{{ TasksList.text }}</h3>
</template>

<script>
export default {
  name: "TasksList",
  props: {
    task: Object,
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
