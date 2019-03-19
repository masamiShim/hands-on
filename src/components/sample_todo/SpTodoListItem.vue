<template>
  <div>
    <div>
      <span v-if="task.done">済</span>
      <span v-else>未</span>
      {{ task.label }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'SpTodoListItem',
  props: {
    task: {
      type: Object,
      required: true
    }
  }
}
</script>

<style scoped>

</style>
