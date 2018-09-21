<template>
  <div class="menu" id="post">
    <div class="item current">
    </div>
    <div class="item page" id="home">
      <house-outline-svg/>
    </div>
    <div class="item current" id="profile">
    </div>
  </div>
</template>

<script>
import ATextBox from '@/components/atoms/a-text-box';
import AH1 from '@/components/atoms/a-h1';
import HouseOutlineSvg from '@/assets/house-outline.svg';

export default {
  name: 'MenuMobile',
  components: {
    ATextBox,
    AH1,
    HouseOutlineSvg,
  },
  props: {
    page: String,
  },
  mounted() {
    const home = document.getElementById('home');
    const post = document.getElementById('post');
    const profile = document.getElementById('profile');
    if (this.page === 'home') {
      home.classList.add('current');
    } else if (this.page === 'post') {
      post.classList.add('current');
    } else if (this.page === 'profile') {
      profile.classList.add('current');
    }
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
  background-color: #fff;
  border-top: 1px solid rgba(0, 0, 0, 0.15);
}
.item {
  padding: 0.5rem 0;
}

.page {
  svg {
    width: 2rem;
    height: 2rem;
  }
  &.not-current {
    svg {
      fill: #ccc;
    }
  }
  &.current {
    h1 {
      color: #7e5ecb;
    }
    svg {
      fill: #7e5ecb;
    }
  }
}
</style>
