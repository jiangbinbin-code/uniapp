<template>
    <view>  
	<!-- 搜索  -->
	<Search>搜索</Search>
	<!-- 轮播  -->
	<Swipers>轮播</Swipers>
	<!-- 抢购  -->
	<Purchase>抢购</Purchase>
	<!-- 榜单  -->
	<List>榜单</List>
	<!-- 卡片  -->
	<Commodity>卡片</Commodity>
	</view>
</template>

<script>
import Search  from './component/search.vue'
import Swipers  from './component/swiper.vue'
import Purchase  from './component/purchase.vue'
import List  from './component/list.vue'
import Commodity  from './component/commodity.vue'
export default{
	//注册进父组件
	components:{Search,Swipers,Purchase,List,Commodity}
}

</script>

<style>
	
</style>
