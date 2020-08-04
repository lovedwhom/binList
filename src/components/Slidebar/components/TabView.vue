<template>
  <div class="tab-view">
    <div class="tab-view-container" >
      <div v-for="(item,index) in list"
           :class="[{active:index ===active},'tab-view-item']"
           :key="index"
          @click="handleClick(index)"
      >{{item.name}}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TabView',
  data () {
    return {
      active: 0,
      list: [
        {
          name: '清单'
        }, {
          name: '标签'
        }
      ]
    }
  },
  methods: {
    handleClick (index) {
      this.active = index
      console.log(111)
    }
  }
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
