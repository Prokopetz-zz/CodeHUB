<template>
  <div class="index">
    <o-header></o-header>
    <a-card></a-card>
    <m-footer page="home"/>
  </div>
</template>

<script>
import ACard from '@/components/atoms/a-card';
import MFooter from '@/components/molecules/m-footer';
import OHeader from '@/components/organisms/o-header';

export default {
  name: 'Index',
  components: {
    ACard,
    MFooter,
    OHeader,
  },
};
</script>

<style scoped lang="stylus">

</style>
