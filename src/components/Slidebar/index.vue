<template>
  <div class="slide-bar border1px">
    <slide-bar-menu></slide-bar-menu>
    <tab-view></tab-view>
    <div></div>
  </div>

</template>

<script>
import SlideBarMenu from './components/SlidebarMenus'
import TabView from './components/TabView'
export default {
  components: {
    SlideBarMenu,
    TabView
  },
  name: 'slidebar'
}
</script>

<style scoped lang="scss">
@import '~@/assets/base.scss';
.slide-bar{
  cursor: pointer;
  padding-bottom: -9999px;
}
</style>
