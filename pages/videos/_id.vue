<template>
	<div>
		<nuxt-child :video='video' />
	</div>
</template>

<script>
	import { mapState } from 'vuex'

	export default {
		head() {
			return {
				title: this.video.name
			}
		},

		async asyncData({ $axios, params, store }) {
			let response = await $axios.get('/videos')
			let videos = response.data.data.map(v => v.attributes)

			store.commit('SET_CURRENT_VIDEO', video)
		},

		computed: {
			...mapState ({
				video: 'currentVideo'
			})
		}
	}
</script>

<style lang="scss" scoped>

</style>