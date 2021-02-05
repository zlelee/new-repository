<template>
  <div id="app">
    <child1 />
    <child2 />
  </div>
</template>
<script>
import child1 from '@/components/child1.vue'
import child2 from './components/child2.vue'
export default {
  name: 'app',
  data() {
    return {
      msg: '你好'
    }
  },
  components: {
    child1,
    child2
  },
  methods: {}
}
</script>
<style>
div {
  height: 200px;
  text-align: center;
}
</style>
