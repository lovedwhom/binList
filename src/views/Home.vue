<template>
  <div class="home-container">
    <div class="sidebar-container">
      <slidebar-menus></slidebar-menus>
    </div>
    <div class="main-container">
      main
    </div>
  </div>
</template>

<script>
import SlidebarMenus from '@/components/SlidebarMenus'
export default {
  name: 'Home',
  components: {
    SlidebarMenus
  }
}
</script>

<style scoped lang="scss">
  .home-container{
    display: flex;
    .sidebar-container{
      width: 300px;
    }
    .main-container{
      flex: 1;
    }
  }
</style>
