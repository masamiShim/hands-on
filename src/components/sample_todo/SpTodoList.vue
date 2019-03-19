<template>
  <ul>
    <li v-for="item in tasks" :key="item.id">
      <SpTodoListItem :task="item" />
    </li>
  </ul>
</template>

<script>

import SpTodoListItem from './SpTodoListItem'
export default {
  name: 'SpTodoList',
  components: { SpTodoListItem },
  props: {
    tasks: {
      type: Array,
      required: true
    }
  }
}
</script>

<style scoped>

</style>
