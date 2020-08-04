<template>
  <div class="badge">
    {{value}}
  </div>
</template>

<script>
export default {
  props: {
    value: {
      type: Number,
      default: 0
    }
  },
  name: 'bin-badge'
}
</script>

<style scoped lang="scss">
.badge{
  float: right;
  //border: 1px solid grey;
  color: #ffffff;
  padding: 0 5px;
  background-color: #409eff;
  border-radius: 10px;
}
</style>
