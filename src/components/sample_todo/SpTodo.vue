<template>
  <div>
    <h1>Todo Sample</h1>
    <SpTodoCreator @add-task="addTask" />
    <SpTodoList :tasks="todo" />
  </div>
</template>

<script>
import SpTodoCreator from './SpTodoCreator'
import SpTodoList from './SpTodoList'
export default {
  name: 'SpTodo',
  components: {SpTodoCreator, SpTodoList},
  data () {
    return {
      todo: [
        { id: 1, label: 'hogehogefuga', done: false }
      ]
    }
  },
  methods: {
    addTask (txt) {
      this.todo.push({ id: this.todo.length + 1, label: txt, done: false })
    }
  }
}
</script>

<style scoped>

</style>
