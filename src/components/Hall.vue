<template>
  <top-bar></top-bar>
  <group title="cell demo">
    <cell title="Vux" value="Cool" is-link></cell>
  </group>
</template>

<script>
import Group from 'vux/src/components/group'
import Cell from 'vux/src/components/cell'
import TopBar from '../TopBar'
import {Divider,FlexboxItem,Flexbox} from 'vux/src/components'

export default {
  components: {
    Group,
    Cell,
    TopBar
  },
  data () {
    return {
      // note: changing this line won't causes changes
      // with hot-reload because the reloaded component
      // preserves its current state and we are modifying
      // its initial state.
      msg: 'Hello World!'
    }
  }
}
</script>

<style>
.vux-demo {
  text-align: center;
}

.logo {
  width: 100px;
  height: 100px
}
</style>
