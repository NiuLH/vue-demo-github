<template>
  <div class="hello">
    姓名：{{name}}
    年龄：{{age}}
    工作：{{info.work}}
    <div><button @click="change">改变</button></div>
  </div>
</template>

<script>
import {ref,reactive} from 'vue'
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  setup(){
    let name=ref('zs');
    let age=ref(18);
    let info=reactive({
      work:"font"
    })
    function change(){
      name.value='ls';
      age.value=20;
      info.work="after"
    }
    return{
      name,
      age,
      info,
      change
    }
  }
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
