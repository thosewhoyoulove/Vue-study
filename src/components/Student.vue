<template>
  <div class="student">
      <h2>学生姓名：{{name}}</h2>
      <h2>学生性别：{{sex}}</h2>
  </div>
</template>

<script>
export default {
    name:'Student',
    data() {
        return {
            name:'caojun',
            sex:'男'
        }
    },
   
}
</script>
<style>
.student{
    background-color: tomato;
    padding: 5px;
    margin-top: 30px;
}
</style>
