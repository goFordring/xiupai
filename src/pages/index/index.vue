<template>
  <div class="map">
    <!-- 这是头部 导航栏-->
   <div class="header">
     <wux-row>
       <wux-col span ="2">
         <span class="city">
           <i-icon type ="coordinates" size ="16" color ="#00CA00"></i-icon>
           青岛
         </span>

       </wux-col>
       <wux-col span ="7">
         <van-search placeholder="搜索师傅 服务类别" shape ="round"></van-search>
       </wux-col>
       <wux-col span ="3">
         <ul class="rightNav">
           <li><img src="/static/images/share.png" alt=""></li>
           <li><img src="/static/images/order.png"></li>
           <li><img src="/static/images/person.png"></li>
         </ul>

       </wux-col>
     </wux-row>
   </div>

    <map name="mapbg" class="mapbg">

    </map>
    <cover-view class ="bottom">
      <!--这是底部 总览 -->
       <cover-view class ="site">
         <cover-view class ="region">
           觅云计算科技有限公司
         </cover-view>
         <cover-view class ="detailSite">
           保税港区曼谷路49号
         </cover-view>
         <cover-view class ="rightIcon">

         </cover-view>
       </cover-view>

    </cover-view>
    <cover-view class ="button">
      <button type ="primary">立即找师傅</button>
    </cover-view>
  </div>
</template>

<script>
  export default{


  }
</script>

<style scoped>
  .map{
    width: 100%;
    height: 100vh;
    overflow: hidden;
  }
  .mapbg{
    width: 100%;
    height:100vh;
  }
  .header{
    height: 100rpx;
    width: 100%;
    }

  .header .city{
    height: 100rpx;
    color: #333333;
    font-size: 34rpx;
    line-height: 100rpx;
    margin-left:10rpx;
  }
  .header .rightNav{
    padding-top: 30rpx;
    height:70rpx;
  }
  .header .rightNav li{
     display: inline-block;
     width:45rpx;
     height:45rpx;
     margin-right: 15rpx;
  }
  .header .rightNav li img{
      width: 100%;
      height: 100%;
  }
  .bottom{
    position: absolute;
    bottom:166rpx;
    width: 696rpx;
    margin:0 auto;
    left: 50%;
    transform: translateX(-50%);
    box-shadow:0rpx 0rpx 10rpx 0rpx rgba(0,67,88,0.18);
  }
  .bottom .region{
    height: 64rpx;
    line-height: 64rpx;
    font-size:32rpx;
    color: #333333;
    font-family: "microsoft yahei";
    padding-left:35rpx;
  }
  .bottom .site{
    padding-top: 10rpx;
    height: 118rpx;
    width: 100%;
    border-radius:10rpx;
    background-color: #FFFFFF;
  }
  .bottom .detailSite{
    color: #999999;
    font-size:28rpx;
    font-family: "microsoft yahei";
    padding-left:35rpx;
  }
  .button{
    position: absolute;
    bottom:46rpx;
    width: 696rpx;
    left:50%;
    transform: translateX(-50%);
    box-shadow:0rpx 0rpx 10rpx 0rpx rgba(0,67,88,0.18);
  }
</style>
