<template>
	<v-container>
		<v-row>
			<v-col cols="2">
				<v-sheet rounded="lg">
					<v-divider class="my-2" style="border-color: transparent;"></v-divider>

					<v-img
						lazy-src="evan.jpg"
						max-height="450"
						max-width="450"
						src="/evan.jpg"
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
								<nuxt-link :to='`/summary/${ item.to }`' class="custom-nuxt-link">
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
				field: "Education",
				to: "education"
			},
			{
				field: "Work History",
				to: "work"
			},
			{
				field: "Certification",
				to: "certificate"
			},
			{
				field: "Reference",
				to: "reference"
			}
		],
		model: 0
	}),
}
</script>

<style>
</style>
