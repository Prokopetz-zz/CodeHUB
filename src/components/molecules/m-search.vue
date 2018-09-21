<template>
  <div class="father">
    <div class="son">
      <search-svg/>
    </div>
    <a-input-text text="Pesquisar"></a-input-text>
  </div>
</template>

<script>
import SearchSvg from '@/assets/icons/search.svg';
import AInputText from '@/components/atoms/a-input-text';

export default {
  name: 'MSearch',
  components: {
    AInputText,
    SearchSvg,
  },
};
</script>

<style lang='stylus' scoped>
.father{
  .son{
    svg {
      width: 1.2rem;
      height: 1.5rem;
      fill: rgba(0, 0, 0, 0.65);
    }
    padding: 0 1rem;
    margin-top: 0.17rem;
  }
  display: flex;
  align-items: center;
  justify-content: space-between;
  row-flex-direction: column;
  width: 100%;
}
</style>
