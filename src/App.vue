<template>
  <div id="app">
    <task v-bind:tasks="tasks"></task>
  </div>
</template>

<script>
import Task from "./components/Task";

export default {
  name: "App",
  components: {
    Task,
  },
  data() {
    return {
      tasks: [
        {
          id: 1,
          title: "Walk Dog",
          completed: true,
        },
        {
          id: 2,
          title: "Read Book",
          completed: true,
        },
        {
          id: 3,
          title: "Grocery Shopping",
          completed: false,
        },
        {
          id: 4,
          title: "Water Lawn",
          completed: false,
        },
        {
          id: 5,
          title: "Call Friend",
          completed: false,
        },
      ],
    };
  },
};
</script>