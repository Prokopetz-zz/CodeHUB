<template>
  <div class="menu">
    <div>
      Post
    </div>
    <div>
      Home
    </div>
    <div>
      Settings
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      msg: '',
    };
  },
};
</script>

<style scoped>

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
