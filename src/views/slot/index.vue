<template>
  {{ name }}
  <express v-model:aaa="name">
    <template #one="{age}">
      xxx {{ age }} <br />
    </template>
    <template #two>
      我是插槽2 <br />
    </template>
  </express>
</template>

<script>
import express from './Tin'
export default {
  data () {
    return {
      name: 'lining'
    }
  },
  components: {
    express
  }
}
</script>
<style lang="less" scoped>

</style>
