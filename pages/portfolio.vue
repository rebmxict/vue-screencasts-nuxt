<template>
	<v-container>
		<v-row>
			<v-col cols="2">
				<v-sheet rounded="lg">
					<v-divider class="my-2" style="border-color: transparent;"></v-divider>

					<v-img
						lazy-src="evan.jpg"
						max-height="250"
						max-width="250"
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
								<v-list-item-content>
									<v-list-item-title>
										{{ item.field }}
									</v-list-item-title>
								</v-list-item-content>
							</v-list-item>
						</v-list-item-group>

						<v-divider class="my-2"></v-divider>

						<v-list-item
							link
							color="grey lighten-4"
						>
							<v-list-item-content>
								<v-list-item-title>
									Refresh
								</v-list-item-title>
							</v-list-item-content>
						</v-list-item>
					</v-list>
				</v-sheet>
			</v-col>

			<v-col>
				<v-sheet
					min-height="70vh"
					rounded="lg"
				>
					Summary page
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
				field: "Project 1",
				to: "/1"
			},
			{
				field: "Project 2",
				to: "/2"
			},
			{
				field: "Project 3",
				to: "/3"
			},
			{
				field: "Project 4",
				to: "/4"
			}
		],
		model: 0
	}),
}
</script>

<style>
</style>
