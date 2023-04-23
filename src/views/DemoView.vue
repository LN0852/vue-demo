<template>
  <div>
    <p v-if="a === 'a'"> A </p>
    <p v-else> B </p>
    <p v-show="a === 'a'"> A Show</p>
    <p v-show="a === 'b'"> B Show</p>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const a = ref('a')
</script>
<style lang="less" scoped>

</style>
