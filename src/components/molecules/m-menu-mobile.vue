<template>
  <div class="menu">
    <div class="item">
      Post
    </div>
    <div class="item">
      Home
    </div>
    <div class="item">
      Settings
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
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
  .item {
    padding: 20px 0px;
  }
}
</style>
