<!--  -->
<template>
  <div>
      <SlotChild>
          <template v-slot:test1>
              <h1>插槽1</h1>
          </template>
          <template v-slot:test2>
              <h3>插槽2</h3>
          </template>
      </SlotChild>
  </div>
</template>

<script>
import SlotChild from './SlotChild.vue'
export default {
  components:{SlotChild},
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