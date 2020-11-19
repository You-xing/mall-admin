<template>
  <div class="home">
    <left-menu></left-menu>
    <div :class="{'main-app':true, 'menu-unfold':$store.state.collapsed}">
      <slider-nav></slider-nav>
    </div>
    <router-view></router-view>
  </div>
</template>

<script>
import LeftMenu from './components/LeftMenu.vue';
import SliderNav from './components/SliderNav.vue';

export default {
  data() {
    return {
      // collapsed: true,
    };
  },
  components: {
    LeftMenu,
    SliderNav,
  },
};
</script>

<style lang="less">
@import url("~@/assets/css/home.less");

</style>
