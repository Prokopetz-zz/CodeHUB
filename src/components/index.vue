<template>
  <div class="index">
    <o-header></o-header>
    <m-menu-mobile page="home"/>  
  </div>
</template>

<script>
import MMenuMobile from '@/components/molecules/m-menu-mobile';
import OHeader from '@/components/organisms/o-header';

export default {
  name: 'Index',
  components: {
    MMenuMobile,
    OHeader,
  },
};
</script>

<style scoped>

</style>
