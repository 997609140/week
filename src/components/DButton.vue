<!--底部确定按钮

<d-button @click="submit">确认添加</d-button>

-->
<template>
  <span
    class="btn"
    @click="click"
  >
    <slot>确认</slot>
  </span>
</template>

<script>
export default {
  name: 'DButton',
  props: {
    // disabled: {
    //     type: Boolean,
    //     default: false
    // }
  },
  methods: {
    click () {
      this.$emit('click')
    }
  }

}
</script>

<style lang="scss" scoped>
    @import "../scss/style";

    .btn {
        margin-top: 60px;
        text-align: center;
        line-height: 100px;
        color: $c-white;
        font-size: 36px;
        border-radius: 4px;
    }

</style>
