<template>
  <div class="father">
    <a-icon></a-icon>
    <a-input-text text="Pesquisar"></a-input-text>
  </div>
</template>

<script>
import AInputText from '@/components/atoms/a-input-text';
import AIcon from '@/components/atoms/a-icon';

export default {
  name: 'MSearch',
  components: {
    AInputText,
    AIcon,
  },
};
</script>

<style lang='stylus' scoped>
.father{
  display: flex;
  align-items: center;
  row-flex-direction: column;
}
</style>
