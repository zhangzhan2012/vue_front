<template>
  <div class="y-wrap">
    <!--    <iframe src="src/components/page/mainPage"></iframe>-->

    <div style="padding-bottom: 0px">
      <img src="../../static/img/表单1.jpg" height="794" width="550"/>
    </div>
    <div class="video-wrap" style="width:80%;float:left;oveflow:hidden;padding-top: 0px;margin-top: -2px">
      <iframe src="../../static/img/表单2.mp4" frameborder='0'
              allow='autoplay;encrypted-media' allowfullscreen style='width:550px;height:309.38px;padding-top: -2px'>
      </iframe>
    </div>
    <div class="stream-frame_963b1" style="">
      <img src="../../static/img/表单3.jpg" height="198.02" width="533"/>
    </div>
    <div class="" style="width:550px;height:50px;text-align: center">
      <div class="ling" style="text-align: center;height: 40px;width: 96%">
        <span>
          <svg class="icon svelte-soflc2" style=" width: 20px;height: 20px;color: red"
               viewBox="0 0 22 20" xmlns="http://www.w3.org/2000/svg"><path
            d="M16.106 13.214c-.342-.396-.334-.856.005-1.216.59-.626.915-1.448.915-2.32 0-.875-.328-1.7-.92-2.326a.93.93 0 0 1 .014-1.283c.349-.35.827-.119.95.014a5.194 5.194 0 0 1 1.421 3.595 5.202 5.202 0 0 1-1.412 3.585c-.172.184-.771.184-.973-.049zm-2.604 6.146c-.19 0-.379-.047-.553-.142L4.403 14.52H1.174C.525 14.52 0 13.976 0 13.31V6.05c0-.669.525-1.21 1.174-1.21h3.229L12.949.142c.365-.199.803-.19 1.158.03.353.218.569.613.569 1.038v16.94c0 .425-.216.82-.569 1.037a1.172 1.172 0 0 1-.605.173zM1.324 13.08h3.372c.193 0 .383.05.553.143l8.09 4.547V1.576L5.248 6.09c-.17.095-.36.142-.553.142H1.324v6.849zm2.838-7.456h1.236v8.408H4.162V5.624zm13.299 11.254c-.298-.394-.097-.974.286-1.283a7.52 7.52 0 0 0 1.702-1.925 7.669 7.669 0 0 0 1.13-4.03c0-2.319-1.016-4.476-2.784-5.917-.38-.311-.489-.873-.188-1.265.226-.234.787-.207.963-.067C20.743 4.431 22 6.805 22 9.681c0 2.906-1.28 5.598-3.51 7.386-.257.206-.86.072-1.029-.19z"
            fill="currentColor" fill-rule="nonzero"></path></svg></span>
        <span class="prefix" style="font-size: 20px">截止目前已有</span>
        <span class="number svelte-soflc2">13498</span>
        <span class="suffix" style="font-size: 20px">名用户参加</span>
      </div>
    </div>
    <div class="submitA">
      <span class="submitB">参与新品特惠</span>
    </div>
    <div>
      <img src="../../static/img/表单4.jpg" height="560" width="550px"/>
      <img src="../../static/img/表单5.jpg" height="794" width="550px"/>
      <img src="../../static/img/表单6.jpg" height="1000px" width="550px"/></div>
      <img src="../../static/img/表单7.jpg" height="360px" width="550px"/>
      <img src="../../static/img/表单8.jpg" height="1100px" width="550px"/>
      <img src="../../static/img/表单9.jpg" height="618px" width="550px"/>
      <img src="../../static/img/表单10.jpg" height="560px" width="550px"/>
    <div style="height: 600px">

    </div>
  </div>
</template>
<script>
//引入video样式

export default {
  data() {
    return {
      playerOptions: {
        playbackRates: [0.7, 1.0, 1.5, 2.0], //播放速度
        autoplay: false, //如果true,浏览器准备好时开始回放。
        controls: true, //控制条
        preload: 'auto', //视频预加载
        muted: false, //默认情况下将会消除任何音频。
        loop: false, //导致视频一结束就重新开始。
        language: 'zh-CN',
        aspectRatio: '16:9', // 将播放器置于流畅模式，并在计算播放器的动态大小时使用该值。值应该代表一个比例 - 用冒号分隔的两个数字（例如"16:9"或"4:3"）
        fluid: true, // 当true时，Video.js player将拥有流体大小。换句话说，它将按比例缩放以适应其容器。
        sources: [{
          type: 'video/mp4',
          src: ''//你所放置的视频的地址，最好是放在服务器上
        }],
        poster: "http://39.106.117.192:8080/static/indexImg.png", //你的封面地址（覆盖在视频上面的图片）
        width: document.documentElement.clientWidth,
        notSupportedMessage: '此视频暂无法播放，请稍后再试' //允许覆盖Video.js无法播放媒体源时显示的默认信息。
      }
    }
  }
}
</script>
<style>

.y-wrap {
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  width: 415px;
  height: 100%;
  margin: 0 auto;
  -webkit-border-radius: 4px;
  border-radius: 4px;
  box-shadow: 2px 3px 10px #999;
}

.y-wrap > iframe {
  background: #eee;
  width: 100%;
  border: none;
}

.number.svelte-soflc2 {
  font-weight: bold;
  font-size: 27px;
  color: #D0021B;
}

.ling {
  border-radius: 40px 40px;
  box-shadow: 2px 3px 10px #999;
  width: 96% !important;
  position: absolute;
}

.submitB {
  margin-top: 10px;
  margin-left: 20%;
  text-align: center;
  height: 50px;
  border-radius: 15px 15px;
  box-shadow: 2px 3px 10px #999;
  background-color: red;
  color: white;
  width: 400px;
  display: block;
}

.submitA {
  position: relative;
  text-align: center;
}

</style>
