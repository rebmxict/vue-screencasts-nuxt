<template>
	<v-card
		class=""
		max-width="100%"
		outlined
		style="margin: 10px;"
	>
		<v-list-item three-line>
			<v-list-item-content style="display: block;">
				<v-btn class="ma-2" color="secondary">React Native</v-btn>
				<v-btn class="ma-2" color="secondary">Ionic</v-btn>
				<v-btn class="ma-2" color="secondary">Flutter</v-btn>
				<v-btn class="ma-2" color="secondary">METEOR</v-btn>
			</v-list-item-content>
		</v-list-item>
	</v-card>
</template>

<script>
	export default {
		data: () => ({
		}),
		methods: {
		}
	}
</script>

<style scoped>
.v-application .secondary {
	background-color: #5cbbf6 !important;
	border-color: #5cbbf6 !important;
}
</style>