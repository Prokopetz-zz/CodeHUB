<template>
    <h1 :style="{'color': color, 'font-size': size }">
      <slot></slot>
    </h1>
</template>

<script>
export default {
  name: 'ATextBox',
  props: {
    color: String,
    size: String,
  },
};
</script>

<style lang='stylus' scoped>

</style>
