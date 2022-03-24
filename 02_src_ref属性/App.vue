<template>
  <div>
    <h1 v-text="msg" ref="title"></h1>
    <button ref="btn" @click="ShowDom">点我</button>
      <School ref="sch"></School>
  </div>
</template>

<script>
import School from './components/School'
export default {
  /**
   * ref 属性 
   *    -被用来给元素或子组件注册引用信息(id的替代者)
   *    - 应用在HTML标签上获取的是真实dom元素，应用在组件标签上是组件实例对象(vc)
   *    - 使用方式：
   *      - 打标识：<h1 ref = "xxx">...</h1>或<School ref = "xxx"></School>
   *      - 获取：this.$refs.xxx
   */
  
    name:'App',
    data() {
      return {
            msg:'HelloWorld!'
      }
    },
    components:{School},
    methods: {
      ShowDom(){
        // console.log(this.$refs.title)
        // console.log(this.$refs.btn)
        console.log(this.$refs.sch)
      }
    },


}
</script>
