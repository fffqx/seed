<template>
	<view>
		<view class="content">
			<van-row>
				<van-col span="16">
					<view class="place" @click="regps()">
						<van-icon name="location-o" custom-style=" font-weight: 700" size="20px" />
						<text>银座商城(和谐广场店)</text>
						<van-icon name="arrow" size="10px" />
					</view>

				</van-col>
			</van-row>
		</view>
		<!-- 搜索 -->
		<view class="search">
			<van-row>
				<van-col>
					
				</van-col>
			</van-row>
		</view>


	</view>
</template>

<script>
	export default {
		data() {
			return {

			}
		},
		onLoad() {

		},
		methods: {
			regps(){
				uni.chooseLocation()
			}
		}
	}
</script>

<style>
	.content {
		background-image: linear-gradient(to right, #FFD44D, #FFC64C);
		height: 100px;
	}

	.place {
		padding: 33px 5px 33px 15px;
		display: flex;
		align-items: center;

	}

	.search {
		background-image: linear-gradient(#FCFCFD, #F5F4F6);
		padding: 0 20px;
		border-radius: 20px 20px 0 0;
		margin-top: -40px;
		min-height: 100px;
	}
</style>
