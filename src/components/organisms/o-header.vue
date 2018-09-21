<template>
  <div class="header">
    <m-search></m-search>
    <a-icon></a-icon>
  </div>
</template>

<script>
import MSearch from '@/components/molecules/m-search';
import AIcon from '@/components/atoms/a-icon';

export default {
  name: 'OHeader',
  components: {
    MSearch,
    AIcon,
  },
};
</script>

<style scoped lang="stylus">
.header {
  display: flex;
  align-items: center;
  justify-content: space-around;
  position: fixed;
  top: 0;
  left: 0;
  right:0;
  box-shadow: 1px 1px 10px grey;
}
</style>
