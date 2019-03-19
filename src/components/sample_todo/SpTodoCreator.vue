<template>
  <div>
    <input type="text" v-model="txt" @keydown.alt.enter="add" />
    <span v-show="hasError">入力してちょ</span>
  </div>
</template>

<script>
export default {
  name: 'SpTodoCreator',
  data () {
    return {
      txt: '',
      hasError: false
    }
  },
  methods: {
    add () {
      if (this.txt.length < 1) {
        this.hasError = true
        return
      }
      this.hasError = false
      this.$emit('add-task', this.txt)
      this.txt = ''
    }
  }
}
</script>

<style scoped>

</style>
