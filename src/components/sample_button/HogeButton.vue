<template>
  <div>
    <button @click="hoge()">say!!</button>
  </div>
</template>

<script>
export default {
  name: 'HogeButton',
  props: {
    message: {
      type: String,
      required: true
    }
  },
  methods: {
    hoge () {
      alert(`Say ${this.message} !! ButtonComponent`)
    }
  }

}
</script>

<style scoped>

</style>
