<template>
  <div id="app">
    <h1>ToDo App</h1>
    <div class="todo-wrapper">
      <div class="todo-container">
        <div class="todo-list">
          <div class="todo-item">
            <div class="todo-item-content">
              <div class="todo-item-title">
                Walk
              </div>
              <div class="todo-item-description">
                Go to Forest
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'App',
    data() {

    },
    components: {

    },
  }
</script>

<style lang="scss" >
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

  .todo{
    &-wrapper{
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
  &-item{
    background-color: #2c3e50;
    min-height: 70px;
    margin: 10px;
    padding: 10px;
    color: #fff;
    border-radius: 10px;
    font-size: 23px;
  }

  &-item-title{
    font-weight: bold;
  }

  &-item-description{
    font-size:19px;
  }

  }
</style>