<template>
    <div :class="{'border' : border}">
      <slot></slot>
    </div>
</template>

<script>
export default {
  name: 'ATextBox',
  props: {
    border: Boolean,
  },
};
</script>

<style lang='stylus' scoped>
div{
    padding: 20px 0;
}
.border {
    border: 2px solid #4C3C1B;
}
</style>
