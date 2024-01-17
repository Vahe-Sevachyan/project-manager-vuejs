<template>
  <div class="container">
    <HeaderMain title="Project Manager" />
    <SetTasks />
  </div>
</template>

<script>
import HeaderMain from "./components/HeaderMain";
import SetTasks from "./components/SetTasks";
export default {
  name: "App",
  components: {
    HeaderMain,
    SetTasks,
  },
  data() {
    return {
      tasks: [],
    };
  },
  created() {
    this.task = [
      {
        id: 1,
        text: "Get better at vue",
        day: "March 1st at 2:30pm",
        reminder: true,
      },
      {
        id: 2,
        text: "Practice VueJS",
        day: "February 13th at 12:30pm",
        reminder: true,
      },
      {
        id: 3,
        text: "Master VueJS",
        day: "April 2nd at 5:30pm",
        reminder: true,
      },
      {
        id: 5,
        text: "Finish the VueJs Course",
        day: "December 13st at 5:30pm",
        reminder: true,
      },
    ];
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@300;400&display=swap");

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: "Poppins", sans-serif;
}

.container {
  max-width: 500px;
  margin: 30px auto;
  overflow: auto;
  min-height: 300px;
  border: 1px solid steelblue;
  padding: 30px;
  border-radius: 5px;
}

.btn {
  display: inline-block;
  background: #000;
  color: #fff;
  border: none;
  padding: 10px 20px;
  margin: 5px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: inherit;
}

.btn:focus {
  outline: none;
}

.btn:active {
  transform: scale(0.98);
}

.btn-block {
  display: block;
  width: 100%;
}
</style>
