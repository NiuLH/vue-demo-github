<template>
  <div class="hello">
    <div>姓名：{{person.name}}</div>
    <div>年龄：{{person.age}}</div>
    <div><button @click="change">改变</button></div>
  </div>
</template>

<script>
import {reactive} from 'vue'
export default {
  name: 'HelloWorld',
  setup(){
    let person=reactive({
      name:'zs',
      age:12
    });
    function change(){
      person.name='ls';
      person.age=21;
    }
    return{
      person,
      change
    }
  }
  
}
</script>
