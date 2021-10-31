<template>
	<!-- <view >
		 左右滑块组件 
		<swiper class="swiper" :indicator-dots="true"  indicator-color="Color: rgba(0,0,0,3)":autoplay="true">
           <swiper-item>
			   <view class="swiper-item uni-bg-red">A </view>
		   </swiper-item>	   
		<swiper-item>
			   <view class="swiper-item uni-bg-green">B </view>
		</swiper-item>
		<swiper-item>
			   <view class="swiper-item uni-bg-blue">C </view>
		</swiper-item>
		</swiper>		
 	</view>	 -->
	<view class = "swiper-top">
	   <view>
		   <swiper :autoplay="false" :corcular = "true" :interval="2000" :duration="1000" > <!-- @change="swiperfun"-->
               <!-- <block v-for="(item,index) in bannerdata" :key="index">
			       <swiper-item>
					   <view class="swiper-item" @click="deTails(item._id)">
						    <image :src="http://h/thexxdd.cn/video/tianmao/001.png" mode ="aspectFill"></image>
					   </view>	       
				   </swiper-item>    
				</block>	 -->	
				<swiper-item>
									   <view class="swiper-item" >
										    <image src="http://h/thexxdd.cn/video/tianmao/001.png"></image>
									   </view>	       
				</swiper-item> 
				<swiper-item>
									   <view class="swiper-item" >
										    <image src="http://h/thexxdd.cn/video/tianmao/001.png"></image>
									   </view>	       
				</swiper-item> 
				<swiper-item>
									   <view class="swiper-item" >
										    <image src="http://h/thexxdd.cn/video/tianmao/001.png"></image>
									   </view>	       
				</swiper-item> 
				<swiper-item>
									   <view class="swiper-item" >
										    <image src="http://h/thexxdd.cn/video/tianmao/001.png"></image>
									   </view>	       
				</swiper-item> 
				<swiper-item>
									   <view class="swiper-item" >
										    <image src="http://h/thexxdd.cn/video/tianmao/001.png"></image>
									   </view>	       
				</swiper-item> 
		   </swiper>
	   </view>
	   <!-- 指示点-->
	   <view class ="instruct-view">
		 <!--  <block v-for="(item,index) in bannerdata" :key="index"> -->
		   <view class ="instruct" ><!-- {{}} --></view><!-- :class="{active:index ==num}" -->
		   
		 <!--  </block> -->
	   </view>
	   
	</view>
</template>

<script>
	export default{
     data(){
		 return{
			 
		 }
	 },
	 created(){
		 this.banner();
	 },
	 methods:{
		 banner(){
			 console.log('123');
		 } 
	 }
	}
	
</script>

<style scoped>
.swiper-top{
	height: 250upx;
	margin: 20upx 10upx;
	border-radius: 10upx;
	posotion: relative; 
	
}

	
swiper{
	height: 250upx !important;
	background: yellow;
	border-radius: 10upx;
	overflow:hidden;
	
}	
.swiper-item{
	height: 250upx !important;
    overflow: hidden;	
	
}	
.swiper-item image{
	width: 100%;
	height: 250upx !important;
    border-radius: 10upx;
		
}	
.instruct-view{
	display: flex;
	justify-content: center;
	position: absolute;
	bottom: 10upx;
	left: 0;
	width: 100%;
}
.instruct{
	backgroud: #4e99ab;
	height: 10upx;
	width: 30upx;
	border-radius: 50upx;
	margin: 0 10upx;
}
.active{
	background: #FFFFFF !important;
}
</style>
