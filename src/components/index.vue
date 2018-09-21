<template>
  <div class="index">
    <o-header></o-header>
    <m-footer page="home"/>  
  </div>
</template>

<script>
import MFooter from '@/components/molecules/m-footer';
import OHeader from '@/components/organisms/o-header';

export default {
  name: 'Index',
  components: {
    MFooter,
    OHeader,
  },
};
</script>

<style scoped>

</style>
