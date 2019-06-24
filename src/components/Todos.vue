<template>
  <div>
    <div v-bind:key="todo.id" v-for="todo in todos">
      <ToDoItem v-bind:todo="todo"/>
    </div>
  </div>
</template>

<script>
import ToDoItem from "@/components/ToDoItem";

export default {
  name: "Todos",
  components: {
    ToDoItem
  },
  props: ["todos"]
};
</script>

<style scoped>
</style>

