<template>
  <header>
    <h1>{{ title }}</h1>
    <AddTaskBtn />
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
}
</style>
