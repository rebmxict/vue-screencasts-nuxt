<template>
	<div>
		<nuxt-child :video='video' />
	</div>
</template>

<script>
	export default {
		head() {
			return {
				title: this.video.name
			}
		},

		async asyncData({ $axios, params }) {
			let response = await $axios.get('/videos')
			let videos = response.data
			let video = {}
			videos.map(_video => {
				if (_video.id === params.id) {
					video = _video
				}
			})
			return { video };
		}
	}
</script>

<style lang="scss" scoped>

</style>