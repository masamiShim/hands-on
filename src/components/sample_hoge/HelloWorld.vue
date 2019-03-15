<template>
  <div class="hello">
    <div>
      <input v-model="msg" />
    </div>
    <span>{{ hello() }}</span>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: ''
    }
  },
  methods: {
    hello () {
      if (this.msg.length === 0) {
        return ''
      }
      return `Hello ${this.msg}`
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
