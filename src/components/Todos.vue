<template>
    <div>
        <div v-for="todo in todos" v-bind:key="todo">
        <h3> {{todo.title}} </h3>

         <TodoItem />  
        </div>
    </div>
</template>

<script>
import TodoItem from './TodoItem.vue';

export default {
    name: "Todos",
    components: {
        TodoItem
    },
    props:["todos"]
    
}
</script>

<style scoped>

</style>