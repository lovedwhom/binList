<template>
  <div class="home-container">
    <div class="sidebar-container">
      <slidebar></slidebar>
    </div>
    <div class="main-container">
      main
    </div>
  </div>
</template>

<script>
import Slidebar from '@/components/Slidebar'
export default {
  name: 'Home',
  components: {
    Slidebar
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
