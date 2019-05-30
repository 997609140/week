<template>
  <div>
    <list>
      <cell
        v-for="(num, index) in lists"
        :key="index"
      >
        <text>{{num}}</text>
      </cell>
    </list>
    <d-button
      class="btn"
    />
  </div>
</template>

<script>
import vue from 'Vue'
import DButton from './DButton'
export default {
  name: 'HelloWorld',
  components: {
    DButton
  },
  data () {
    return {
      key: 2,
      lists: ['A', 'B', 'C', 'D', 'E']
    }
  },
  created (e) {
    console.log(e)
  }
}
</script>

<style lang="scss" scoped>
    @import '../scss/style.scss';
    .message {
      color: aqua
    }
    .messaget {
      color: antiquewhite
    }
    .btn {
        background-color: $c-theme;
    }
</style>
