<template>
  <div class="slideMenus border1px">
    <ul>
      <li>
        <base-menu class="22">22</base-menu>
      </li>
      <li>1</li>
      <li>1</li>
      <li>1</li>
      <li>1</li>
      <li>1</li>
      <li>1</li>
      <li>1</li>
      <li>2</li>
    </ul>
  </div>
</template>

<script>
import BaseMenu from '@/components/baseComponent/BaseMenu/index'
export default {
  name: 'slideMenus',
  components: { BaseMenu }
}
</script>

<style scoped lang="scss">
.slideMenus{
  padding-bottom: 9999px;
}
</style>
