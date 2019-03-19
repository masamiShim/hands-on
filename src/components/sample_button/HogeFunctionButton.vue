<template>
  <div>
    <button @click="message">say!!</button>
  </div>
</template>

<script>
export default {
  name: 'HogeFunctionButton',
  props: {
    message: {
      type: Function,
      required: true
    }
  }
}
</script>

<style scoped>

</style>
