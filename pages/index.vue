<template>
	<div class="container">
		<div class="display-4 ma-4 d-flex justify-center">All Videos</div>

		<div class="d-flex flex-wrap">
			<div v-for="video in videos" :key="video.name">
				{{ video.name }}
				<VideoListVideo :video="video">
					
				</VideoListVideo>
			</div>
		</div>
	</div>
</template>

<script>
import VideoListVideo from '../components/VideoListVideo'
export default {
	components: {
		VideoListVideo
	},

	async asyncData({ $axios }) {
		let response = await $axios.get('/videos')
		let videos = response.data.data.map(v => v.attributes)
		
		return {
			videos
		}
	}
}
</script>

<style>
</style>
