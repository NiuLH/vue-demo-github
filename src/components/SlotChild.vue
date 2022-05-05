<!--  -->
<template>
  <div>
    <slot name="test1"></slot>
    <div>子组件</div>
    <slot name="test2"></slot>
  </div>
</template>

<script>
export default {
  data () {
    return {
    };
  },

  created(){
  },

  methods: {}
}

</script>
<style lang='scss' scoped>
</style>