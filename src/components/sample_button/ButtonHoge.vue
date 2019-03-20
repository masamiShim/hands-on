<template>
  <div>
    <div>
      <input v-model="mes" type="text"/>
    </div>
    <HogeButton :message="mes"/>
    <HogeFunctionButton :message="hoge"/>
  </div>
</template>

<script>
// コンポーネントを使う場合はimportする必要あり
// @はwebpackの設定でsrcフォルダからの相対パスとなる
import HogeButton from '@/HogeButton'
import HogeFunctionButton from './HogeFunctionButton'
export default {
  name: 'ButtonHoge',
  components: {HogeButton, HogeFunctionButton},
  data () {
    return {
      mes: ''
    }
  },
  methods: {
    hoge () {
      alert(`Hoge ${this.mes} FunctionProp`)
    }
  }
}
</script>

<style scoped>

</style>
