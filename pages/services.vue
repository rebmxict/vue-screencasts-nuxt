<template>
	<v-container>
		<v-row>
			<v-col cols="2">
				<v-sheet rounded="lg">
					<v-divider class="my-2" style="border-color: transparent;"></v-divider>

					<v-img
						lazy-src="/rio.png"
						max-height="450"
						max-width="450"
						src="/rio.png"
					></v-img>

					<v-list color="transparent">
						<v-list-item-group
							v-model="model"
						>
							<v-list-item
								v-for="item in items"
								:key="item.to"
								link
							>
								<nuxt-link :to='`/services/${ item.to }`' class="custom-nuxt-link">
									<v-list-item-content>
										<v-list-item-title>
											{{ item.field }}
										</v-list-item-title>
									</v-list-item-content>
								</nuxt-link>
							</v-list-item>
						</v-list-item-group>

						<v-divider class="my-2"></v-divider>
					</v-list>
				</v-sheet>
			</v-col>

			<v-col style="">
				<v-sheet
					min-height="0vh"
					rounded="lg"
					style="overflow: hidden;margin-top: 8px;"
				>
					<nuxt-child />
				</v-sheet>
			</v-col>
		</v-row>
	</v-container>
</template>

<script>
export default {
	data: () => ({
		items: [
			{
				field: "Web",
				to: "web"
			},
			{
				field: "Mobile",
				to: "mobile"
			},
			{
				field: "Database",
				to: "database"
			},
			{
				field: "DevOps",
				to: "devops"
			}
		],
		model: 0,
	}),
	mounted () {
		let root = '/services/web'
		this.$router.push({ path: root, query: { } });
	}
}
</script>

<style>
</style>
