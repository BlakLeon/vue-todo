<template>
    <div class="todo-item">
        <div class="todo-item-content">
            <div class="todo-item-title">
                {{title}}
            </div>
            <div class="todo-item-description">
                {{description}}
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        props:['title','description']

    }
</script>

<style lang="scss" scoped>
    .todo {
        &-item {
            background-color: #2c3e50;
            min-height: 70px;
            margin: 10px;
            padding: 10px;
            color: #fff;
            border-radius: 10px;
            font-size: 23px;
        }

        &-item-title {
            font-weight: bold;
        }

        &-item-description {
            font-size: 19px;
        }
    }
</style>