<template>
  <!-- 二级路由的默认组件 -->
  <div class="second-home">
    <!-- 幻灯片 -->
    <el-carousel :interval="4000" type="card" height="300px">
      <el-carousel-item v-for="item in list" :key="item">
        <img :src="item" alt />
      </el-carousel-item>
    </el-carousel>
  </div>
</template>

<script>
export default {
  data () {
    return {
      list: [
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1583648384917&di=6dd93d6fd9e28f6d4de1265b9269d2bc&imgtype=0&src=http%3A%2F%2Fk.zol-img.com.cn%2Fdcbbs%2F11651%2Fa11650421_01000.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1583648505738&di=a29a4015402cfa905a1747a2db62f802&imgtype=0&src=http%3A%2F%2Fimg.pconline.com.cn%2Fimages%2Fupload%2Fupc%2Ftx%2Fphotoblog%2F1105%2F17%2Fc0%2F7685074_7685074_1305568042642.jpg',
        'https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=1179015191,2307410520&fm=26&gp=0.jpg',
        'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1583648821433&di=27c81c3816acb31cfa11727ba893ca5c&imgtype=jpg&src=http%3A%2F%2Fimg4.imgtn.bdimg.com%2Fit%2Fu%3D1417223794%2C1058036723%26fm%3D214%26gp%3D0.jpg'
      ]
    }
  }
}
</script>

<style lang='less'>
.second-home {
  /* calc 计算的意思 在css中计算数值 用法  calc ( 四则运算  ) 变量之间 和运算符之间一定要有空格 */
  height: calc(100vh - 60px);
  background-size: cover;
  background-image: url('https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1583659225944&di=c6cb3b2a292475913d839aeab21767a6&imgtype=0&src=http%3A%2F%2Fpic1.win4000.com%2Fwallpaper%2F2020-02-25%2F5e54b3b2e6213.jpg');
  img {
    width: 100%;
    height: 100%;
  }
}
</style>
