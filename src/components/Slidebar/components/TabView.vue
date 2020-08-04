<template>
  <div class="tab-view">
    <div class="tab-view-container">
      <div class="tab-view-item active">清单</div>
      <div class="tab-view-item">标签</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TabView'
}
</script>

<style scoped lang="scss">
@import "~@/assets/base.scss";
.tab-view{
  padding:$basePadding10  $basePadding20;
  .tab-view-container{
    display: flex;
    justify-content: center;
    align-items: center;
    .tab-view-item{
      line-height: 2em;
      flex: 1;
      border-bottom: $border1solidgGray ;
      &:hover{
        background-color: $hoverBgColor;
      }
      &.active{
        border-bottom: $border1solid ;
      }
    }
  }
}
</style>
