<template>
  <div>
    <ul>
      <li v-for="(item,index)"></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      stu:[{
        name:'zs',
        age:10
      },{
        name:'ls',
        age:30
      },
        {
          name:'ww',
          age:30
        }]
    }
  }
}
</script>
