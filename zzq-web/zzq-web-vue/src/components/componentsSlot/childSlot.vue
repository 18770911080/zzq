<template>    
  <div>
    <!--插槽的应用场景:主要用于多个父组件对于一个字组件的内容有不同的实现方式-->
    <!--匿名插槽-->
    <slot></slot>
    <!--具名插槽-->
    <slot name="test">
      child hello world
    </slot>
    <!--作用域插槽——带数据的插槽-->
    <slot :data="data"></slot>
  </div>
</template>

<script>
  export default {
    data: function(){
      return {
        data: ['zhangsan','lisi','wanwu','zhaoliu','tianqi','xiaoba']
      }
    }
  }
</script>
