<template>
	<v-app id="inspire">
		<v-app-bar
			app
			color="green"
			flat
		>
			<v-container class="py-0 fill-height">
				<v-avatar
					class="mr-10"
					color="grey darken-1"
					size="32"
				>
					<img src="/mark.png" />
				</v-avatar>
				<span style="font-weight: bold">Rio Ephraim</span>

				<v-spacer></v-spacer>

				<v-btn-toggle
					v-model="toggle_exclusive"
					color="primary"
					dense
					mandatory
					group
				>
					<v-btn
						v-for="link in links"
						:key="link.to"
						text
						class="active-class"
					>
						<nuxt-link :to='`${ link.to }`' class="custom-nuxt-link">
							{{ link.field }}
						</nuxt-link>
					</v-btn>
				</v-btn-toggle>
			</v-container>
		</v-app-bar>

		<v-main class="grey lighten-3">
			<Nuxt />
		</v-main>
	</v-app>
</template>

<script>
	export default {
		data: () => ({
			links: [
				{
					field: 'Summary',
					to: '/summary'
				},
				{
					field: 'Services',
					to: '/services'
				},
				{
					field: 'Portfolio',
					to: '/portfolio'
				},
				{
					field: 'Contact',
					to: '/contact'
				}
			],
			model: 0,
		}),
	}
</script>

<style>
.custom-nuxt-link {
	color: #000000db!important;
	text-decoration: none;
	width: 100%;
}

.container {
	max-width: 1178px!important;
}
</style>
