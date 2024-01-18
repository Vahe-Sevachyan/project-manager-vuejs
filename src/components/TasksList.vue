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
