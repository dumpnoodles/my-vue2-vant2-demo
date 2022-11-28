<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <van-button type="primary">主要按钮</van-button>
    <van-button type="info">信息按钮</van-button>
    <van-checkbox v-model="checked">复选框</van-checkbox>



  </div>
</template>

<script>
  import { Button, Checkbox } from 'vant';
export default {
  name: 'HelloWorld',
  data() {
    return {
      checked: true,
    }
  },
  props: {
    msg: String
  },
  components: {
    [Button.name]: Button,
    [Checkbox.name]: Checkbox,
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
