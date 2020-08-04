<template>
  <div class="slideMenus">
    <ul>
      <li v-for="(item,index) in menus" :key="index">
        <base-menu :value="item.count">
          <template slot="title">
            <i :class="['iconfont', item.icon]"></i>
            <span>{{item.label}}</span>
          </template>
        </base-menu>
      </li>
    </ul>
  </div>
</template>

<script>
import BaseMenu from '@/components/baseComponent/menu/index'
import menus from '@/static/menu'
export default {
  name: 'slideMenus',
  components: { BaseMenu },
  data () {
    return {
      menus: menus
    }
  }
}
</script>

<style scoped lang="scss">

.slideMenus{}
</style>
