<template>
  <div>
    <flexbox class="bg-color">
      <flexbox-item>
        <div class="flex-demo">返回</div>
      </flexbox-item>
      <flexbox-item>
        <div class="flex-demo">父母圈</div>
      </flexbox-item>
      <flexbox-item>
        <div class="flex-demo"></div>
      </flexbox-item>
    </flexbox>
  </div>
</template>
<style scoped>
    body{
        background-color:#ff0000;
    }

    .bg-color {
      background-color: #FFFFFF;
    }

   .flex-demo {
      text-align: center;  /*文本居中显示*/
      color: #000;
      background-color: #FFFFFF;
    }
</style>
<script>
import {Divider,FlexboxItem,Flexbox} from 'vux/src/components'

    export default{
        data(){
            return{
            }
        },
        components:{
          Divider,
          FlexboxItem,
          Flexbox
        }
    }

</script>
