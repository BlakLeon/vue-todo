<template>
  <div id="app">
    <h1>ToDo App</h1>
    <div class="todo-wrapper">
      <div class="todo-container">
        <TodoList :todos="todos" />
        <div class="todo-create-btn">
          <div class="app-btn">
            Create
          </div>
        </div>
      </div>
    </div>
    <div class="modal">
      <div class="modal-content">

      </div>
    </div>
  </div>
</template>

<script>

import TodoList from "@/components/TodoList"


  export default {
    name: 'App',
    data() {  
      return{
        todos:[
          {
            _id:"1",
            title:"Walk the Dog",
            description:"Near the zoo"
          },
                    {
            _id:"2",
            title:"Walk the cat",
            description:"Near the zoo"
          },
                    {
            _id:"3",
            title:"Walk the inguana",
            description:"Near the zoo"
          },
        ]
      }

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


  

  .app-btn{
    font-size: 20px;
    padding: 10px;
    border-radius: 5px;
    background-color: #795899;
    color: #fff;
    font-weight: bold;
    &:hober{
      cursor: pointer;
    }
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
      flex-direction: column;
      justify-content: center;
      width: 100%;
      border-radius: 5px;
    }
    &-create-btn{
    margin: 10px;
  }


  }

  .modal{
    display: none;
    position: fixed; //stay in plce
    z-index: 9999;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    overflow: auto;
    background-color: rgba($color: #000000, $alpha: 0.4);
  }
.modal-content{
  background-color: #fefefe;
  margin: 15% auto;
  padding: 20px;
  border: 1px solid #888;
  width: 75%;

}





</style>