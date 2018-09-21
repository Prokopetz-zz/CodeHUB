<template>
  <div class="menu">
    <div class="item">
      <a-h1 size="12px" color="#7e5ecb">News</a-h1>
    </div>
    <div class="item">
      <a-h1 size="12px" color="#7e5ecb">Home</a-h1>
    </div>
    <div class="item">
      <a-h1 size="12px" color="#7e5ecb">Profile</a-h1>
    </div>
  </div>
</template>

<script>
import ATextBox from '@/components/atoms/a-text-box';
import AH1 from '@/components/atoms/a-h1';

export default {
  name: 'MenuMobile',
  components: {
    ATextBox,
    AH1,
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
.item {
  padding: 20px 0;
}
</style>
