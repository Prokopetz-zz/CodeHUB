<template>
  <div class="menu">
    <a-text-box>
      Post
    </a-text-box>
    <a-text-box>
      Home
    </a-text-box>
    <a-text-box>
      Settings
    </a-text-box>
  </div>
</template>

<script>
import ATextBox from '@/components/atoms/a-text-box';

export default {
  name: 'MenuMobile',
  components: {
    ATextBox,
  },
};
</script>

<style scoped lang="stylus">
.menu {
  display: flex;
  align-items: center;
  justify-content: space-around;
  position: fixed;
  bottom: 0;
  left: 0;
  right:0;
}
</style>
