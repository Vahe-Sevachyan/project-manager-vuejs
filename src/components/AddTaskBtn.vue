<template>
  <button v-on:click="onClick" v-bind:style="{ background: color }" class="btn">
    {{ text }}
  </button>
</template>
<script>
export default {
  name: "AddTaskBtn",
  props: {
    text: String,
    color: String,
  },
  methods: {
    onClick() {
      console.log("clicked");
    },
  },
};
</script>
