<template>
    <div class="todo-list">
        <TodoItem :title="'Walk the dog'" :description="'Go to forest and Buy bread'"/>
        <TodoItem :title="todoTitle" :description="todoDesc" />
        
    </div>

</template>

<script>

import TodoItem from "@/components/TodoItem"

    export default {
        components:{
            TodoItem
        },
        data(){
            return{
                todoTitle:"Learn Vue",
                todoDesc:"Vue is the best"
            }
        }

    }
</script>

<style lang="scss" scoped>

</style>