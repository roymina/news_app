<template>
  <div>
    <panel header="图文组合列表" :footer="footer" :list="list" :type="type"></panel>
  </div>
</template>

<script>
import { Panel} from 'vux/src/components'
export default {
  components: {
    Panel
  },
  data () {
    return {
      type: '1',
      list: [{
        src: 'http://placeholder.qiniudn.com/60x60/3cc51f/ffffff',
        title: '标题一',
        desc: '由各种物质组成的巨型球状天体，叫做星球。星球有一定的形状，有自己的运行轨道。',
        url: '/component/cell'
      }, {
        src: 'http://placeholder.qiniudn.com/60x60/3cc51f/ffffff',
        title: '标题二',
        desc: '由各种物质组成的巨型球状天体，叫做星球。星球有一定的形状，有自己的运行轨道。',
        url: {
          path: '/component/radio',
          replace: false
        }
      }],
      footer: {
        title: '查看更多',
        url: 'http://vux.li'
      }
    }
  }
}
</script>
