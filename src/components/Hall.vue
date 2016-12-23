<template>
  <top-bar></top-bar>
  <flexbox class="bg-color">
    <flexbox-item>
      <div class="flex-demo">视频监控</div>
    </flexbox-item>
    <flexbox-item>
      <div class="flex-demo">签到</div>
    </flexbox-item>
    <flexbox-item>
      <div class="flex-demo">发布</div>
    </flexbox-item>
    <flexbox-item>
      <div class="flex-demo">1</div>
    </flexbox-item>
  </flexbox>

  <flexbox class="bg-color">
    <flexbox-item>
      <div class="flex-demo">2</div>
    </flexbox-item>
    <flexbox-item>
      <div class="flex-demo">3</div>
    </flexbox-item>
    <flexbox-item>
      <div class="flex-demo">4</div>
    </flexbox-item>
    <flexbox-item>
      <div class="flex-demo">5</div>
    </flexbox-item>
  </flexbox>

</template>

<script>
import Group from 'vux/src/components/group'
import Cell from 'vux/src/components/cell'
import TopBar from '../TopBar'
import * as GlobalConfig from '../GlobalConfig.js'
import {Divider,FlexboxItem,Flexbox} from 'vux/src/components'

export default {
  components: {
    Group,
    Cell,
    TopBar,
    Divider,
    FlexboxItem,
    Flexbox
  },
  data () {
    return {
      // note: changing this line won't causes changes
      // with hot-reload because the reloaded component
      // preserves its current state and we are modifying
      // its initial state.
      msg: 'Hello World!'
    }
  },
  ready(){
      var requestUrl = GlobalConfig.BASE_URL + GlobalConfig.ATTENDANCE_GET_ALL_LOCATION;
     alert(requestUrl);
  }
}
</script>

<style>


    .bg-color {
      background-color: #FFFFFF;
    }

   .flex-demo {
      text-align: center;  /*文本居中显示*/
      color: #000;
      background-color: #FFFFFF;
    }
</style>
