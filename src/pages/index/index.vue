<template>
  <div class="container">
    <view class="search">
      <!-- 搜索框 -->
      <view class="input-box">
        <input type="text" />
      </view>
      <!-- 搜索结果 -->
      <view class="content"></view>
    </view>
    <swiper>
      <swiper-item>
        <image src="/static/uploads/banner1.png" />
      </swiper-item>
      <swiper-item>
        <image src="/static/uploads/banner2.png" />
      </swiper-item>
      <swiper-item>
        <image src="/static/uploads/banner3.png" />
      </swiper-item>
    </swiper>
    <!-- 导航菜单 -->
    <view class="navs">
      <navigator url>
        <image src="/static/uploads/icon_index_nav_1@2x.png" />
      </navigator>
      <navigator url>
        <image src="/static/uploads/icon_index_nav_2@2x.png" />
      </navigator>
      <navigator url>
        <image src="/static/uploads/icon_index_nav_3@2x.png" />
      </navigator>
      <navigator url>
        <image src="/static/uploads/icon_index_nav_4@2x.png" />
      </navigator>
    </view>
   <view class="floors">
  <view class="floor">
    <!-- 标题 -->
    <view class="title">
      <image src='/static/uploads/pic_floor01_title.png'/>
    </view>
    <!-- 条目 -->
    <view class="items">
      <navigator url=''>
        <image src="/static/uploads/pic_floor01_1@2x.png"></image>
      </navigator>
      <navigator url=''>
        <image src="/static/uploads/pic_floor01_2@2x.png"></image>
      </navigator>
      <navigator url=''>
        <image src="/static/uploads/pic_floor01_3@2x.png"></image>
      </navigator>
      <navigator url=''>
        <image src="/static/uploads/pic_floor01_4@2x.png"></image>
      </navigator>
      <navigator url=''>
        <image src="/static/uploads/pic_floor01_5@2x.png"></image>
      </navigator>
    </view>
  </view>
</view>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: "Hello"
    };
  },
  onLoad() {},
  methods: {}
};
</script>

<style lang='less'>
image{
	display: inline;
}
.search {
  .input-box {
    background-color: #eb4450;
    padding: 20rpx;
    input {
      background-color: #fff;
      border-radius: 6rpx;
    }
  }
}
swiper {
  height: 340rpx;
  image {
    width: 750rpx;
    height: 340rpx;
  }
}
.navs {
  height: 190rpx;
  display: flex;
  justify-content: space-between;
  padding: 0 30rpx;
  align-items: center;
  navigator {
    width: 128rpx;
    height: 140rpx;
    image {
      width: 100%;
      height: 100%;
    }
  }
}
.floor {
  .title {
    width: 750rpx;
    height: 60rpx;
    padding: 20rpx 0 0 10rpx;
    background-color: #f4f4f4;
    image {
      display: inline;
    }
  }
  .items {
    padding: 20rpx 16rpx;
    overflow: hidden;
    navigator {
      float: left;
      margin-left: 10rpx;
      &:first-child {
        width: 232rpx;
        height: 386rpx;
        margin-left: 0;
      }
      &:nth-child(2),
      &:nth-child(5) {
        width: 273rpx;
        height: 188rpx;
      }
      &:nth-child(3),
      &:nth-child(4) {
        width: 193rpx;
        height: 188rpx;
      }
      &:nth-last-child(-n + 2) {
        margin-top: 10rpx;
      }
    }
  }

  &:first-child {
    .items {
      navigator {
        width: 232rpx;
        height: 188rpx;
        &:first-child {
          width: 232rpx;
          height: 386rpx;
        }
      }
    }
  }
}
</style>
