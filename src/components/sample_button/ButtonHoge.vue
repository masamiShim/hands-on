<template>
  <div>
    <div>
      <input v-model="mes" type="text"/>
    </div>
    <div>
      <button @click="hoge()">say!!</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ButtonHoge',
  data () {
    return {
      mes: ''
    }
  },
  methods: {
    hoge () {
      alert(`Say ${this.mes} !!`)
    }
  }
}
</script>

<style scoped>

</style>
