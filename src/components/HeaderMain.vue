<template>
  <header>
    <h1>{{ title }}</h1>
    <AddTaskBtn text="Add Task" color="green" />
  </header>
</template>
<script>
import AddTaskBtn from "./AddTaskBtn.vue";
export default {
  name: "HeaderMain",
  props: {
    title: String,
  },
  components: {
    AddTaskBtn,
  },
};
</script>
<style>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
