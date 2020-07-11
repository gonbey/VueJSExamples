<template>
  <div class="hello">
    <h1>サンプル作成</h1>
    <input v-model="myname" placeholder="入力してください">
    <p>私は、{{ myname }}です</p>
    <p>上記文字列は{{ myname.length }}です</p>
    <label><input type="checkbox" v-model="myCheckbox">チェックボックスは、 {{ myCheckbox }}</label>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      myname: 'テスト文字列',
      myCheckbox: false 
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
