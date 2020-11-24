<template>
  <div class="">
    <h1>HelloWorld</h1>
    <audio src="http://music.163.com/song/media/outer/url?id=276130.mp3" controls="controls">
            您的浏览器不支持 audio 标签。
    </audio> 
    <div class="lrc">
      <el-carousel direction="vertical" :interval="5000" type="" height="100px">
        <el-carousel-item  v-for="item in 56" :key="item">
          <!-- <h3 class="">{{ item }}sdfsdfdsfsdfsd</h3> -->
          <span>sdfsdfsd</span>
        </el-carousel-item>
      </el-carousel>
    </div>
  
  </div>
  
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data:() => ({
    show: true,

  }),
  created(){
    this.loadMusic()
  },
  methods: {
    loadMusic(){
      //POST
      //https://music.liuzhijin.cn/
      //input: 女人花
      //filter: name
      //type: netease
      //page: 1
      /*
        {
          code: 200,
          data: [
            {
              author: "梅艳芳"
              link: "http://music.163.com/#/song?id=276130"
              lrc: ""
              pic: "http://p4.music.126.net/277Ag7Ksu94nhJgXaj2A7Q==/109951163066639996.jpg?param=300x300"
              songid: 276130
              title: "女人花"
              type: "netease"
              url: "http://music.163.com/song/media/outer/url?id=276130.mp3"
            }
          ],
          error:""
        }
      */
      // alert("https://music.liuzhijin.cn/")
    }
  }
}



</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.el-carousel__item h3 {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    line-height: 200px;
    margin: 0;
  }
  
  .el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
  }
  
  .el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
  }
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.transition-box {
    margin-bottom: 10px;
    width: 200px;
    height: 100px;
    border-radius: 4px;
    background-color: #409EFF;
    text-align: center;
    color: #fff;
    padding: 40px 20px;
    box-sizing: border-box;
    margin-right: 20px;
  }
.el-row {
    margin-bottom: 20px;
    &:last-child {
      margin-bottom: 0;
    }
  }
  .el-col {
    border-radius: 4px;
  }
  .bg-purple-dark {
    background: #99a9bf;
  }
  .bg-purple {
    background: #d3dce6;
  }
  .bg-purple-light {
    background: #e5e9f2;
  }
  .grid-content {
    border-radius: 4px;
    min-height: 36px;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }
</style>


/*
  "↵"分割
  [00:00.00]作曲：陈耀川↵
  [00:01.00]作词：李安修↵
  [00:32.03]我有花一朵↵
  [00:35.14]种在我心中↵
  [00:38.54]含苞待放意幽幽↵
  [00:44.40]朝朝与暮暮↵
  [00:47.59]我切切地等候↵
  [00:51.19]有心的人来入梦↵
  [01:00.00]女人花 摇曳在红尘中↵
  [01:06.40]女人花 随风轻轻摆动↵
  [01:12.79]只盼望 有一双温柔手↵
  [01:19.13]能抚慰 我内心的寂寞↵
  [01:26.16]我有花一朵↵
  [01:29.53]花香满枝头↵
  [01:32.60]谁来真心寻芳踪↵
  [01:39.01]花开不多时↵
  [01:42.13]啊堪折直须折↵[01:45.48]女人如花花似梦↵[02:07.56]我有花一朵↵[02:10.90]长在我心中↵[02:14.19]真情真爱无人懂↵[02:20.39]遍地的野草↵[02:23.68]已占满了山坡↵[02:27.30]孤芳自赏最心痛↵[02:32.25]女人花 摇曳在红尘中↵[02:39.16]女人花 随风轻轻摆动↵[02:45.15]只盼望 有一双温柔手↵[02:51.87]能抚慰 我内心的寂寞↵[02:58.31]女人花 摇曳在红尘中↵[03:04.73]女人花 随风轻轻摆动↵[03:10.91]若是你 闻过了花香浓↵[03:17.32]别问我 花儿是为谁红↵[03:28.19]爱过知情重↵[03:31.24]醉过知酒浓↵[03:34.60]花开花谢终是空↵[03:40.82]缘分不停留↵[03:43.80]像春风来又走↵[03:47.33]女人如花花似梦↵[03:53.68]缘分不停留↵[03:56.67]像春风来又走↵[04:00.11]女人如花花似梦↵[04:06.47]女人如花花似梦↵"
*/



