<template>
  <div>
    child2
    {{ msg }}
  </div>
</template>

<script>
import { hub } from '../main.js'

export default {
  name: '',
  data() {
    return {
      msg: 'haa'
    }
  },

  methods: {},
  mounted() {
    hub.$on('changeMsg', (newMsg) => {
      this.msg = newMsg
    })
  }
}
</script>

<style lang="less" scoped></style>
