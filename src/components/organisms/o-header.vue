<template>
  <div class="header">
    <m-search></m-search>
    <div class="svg-box">
      <filter-svg></filter-svg>
    </div>
  </div>
</template>

<script>
import MSearch from '@/components/molecules/m-search';
import FilterSvg from '@/assets/icons/filter.svg';

export default {
  name: 'OHeader',
  components: {
    MSearch,
    FilterSvg,
  },
};
</script>

<style scoped lang="stylus">
.header {
  .svg-box{
    svg {
      width: 1.5rem;
      height: 1.5rem;
      fill: rgba(0, 0, 0, 0.65);
    }
    padding: 0 1rem;
    margin-top: 0.17rem;
  }
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: fixed;
  top: 0;
  left: 0;
  right:0;
  box-shadow: 1px 1px 5px rgba(0,0,0,0.2);
  padding: 5px;
}
</style>
