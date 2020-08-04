<template>
  <div class="base-menu">
      <slot name="title"></slot>
      <badge v-bind="$attrs"></badge>
  </div>
</template>

<script>
import Badge from '@/components/badge'
export default {
  components: {
    Badge
  },
  name: 'bin-menu'
}
</script>

<style scoped lang="scss">
@import '~@/assets/base.scss';
.base-menu{
  cursor: pointer;
  padding: $basePadding10 $basePadding20;
  text-align: left;
  &:hover{
    background-color: $hoverBgColor;
  }
  &> .iconfont{
    margin-right: $basePadding20;
  }

}

</style>
