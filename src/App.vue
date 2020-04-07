<template>
  <div id="app">
    <h1>ToDo App</h1>
    <div class="todo-wrapper">
      <div class="todo-container">
        <TodoList />
      </div>
    </div>
  </div>
</template>

<script>

import TodoList from "@/components/TodoList"


  export default {
    name: 'App',
    data() {

    },
    components: {
      TodoList
    },
  }
</script>

<style lang="scss" scoped >
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

  .todo {
    &-wrapper {
      margin: 0 auto;
      width: 400px;
      min-height: 400px;
      background-color: #ededed;
    }

    &-container {
      display: flex;
      justify-content: center;
      width: 100%;
      border-radius: 5px;
    }

  }
</style>