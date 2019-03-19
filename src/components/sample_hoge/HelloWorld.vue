<template>
  <!-- ここにHTMLを書いてく -->
  <div class="hello">
    <div>
      <!-- v-modelを指定すると値を双方向バインディングしてくれる -->
      <input v-model="msg" />
    </div>
    <!-- {{}}　mustash←で囲むと scriptの要素を表示できる -->
    <span>{{ hello() }}</span>
  </div>
</template>

<script>
export default {
  // コンポーネントの名前
  name: 'HelloWorld',
  // このコンポーネントが保持してるプロパティ
  data () {
    return {
      msg: ''
    }
  },
  // コンポーネントのメソッド, computedもあるけど今回は扱わず
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
