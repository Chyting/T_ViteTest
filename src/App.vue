<template>
  <div>
    <img alt="Vue logo" src="./assets/logo.png" />
<!--    <ul class="li-style">-->
<!--      <li v-for="(stu,index) in student" :key="stu.id">-->
<!--        {{stus.id}} -&#45;&#45;&#45;&#45; {{stus.name}}-->
<!--      </li>-->
<!--    </ul>-->
    <div>{{flag}}</div>
  </div>
</template>

<script>
import {reactive,toRefs} from 'vue'
export default {
  // name: 'App',
  setUp(){
    const state = reactive({
      flag:1
      // student:[
      //   {id:0,name:'zs', age:10},
      //   {id:1,name:'ls', age:30},
      //   {id:2,name:'ww', age:30}
      //   ]
    })
    return { ...toRefs(state) }
  }
}
</script>
<style>
.li-style{
  list-style: none;
  font-size:25px
}
</style>