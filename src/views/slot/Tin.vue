<template>
  <br />
  <slot name="one" :age="age">
    插槽1
  </slot>
  <slot name="two">
    插槽2
  </slot>
  <slot>
    插槽3
  </slot>
  <input type="text" :value="aaa" @input="$emit('update:aaa', $event.target.value)">
</template>

<script>

export default {
  model: {
    prop: 'aaa',
    event: 'change'
  },
  props: {
    aaa: String
  },
  data () {
    return {
      age: 10
    }
  }
}

</script>
