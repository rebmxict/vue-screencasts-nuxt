<template>
	<v-card
		class=""
		max-width="100%"
		outlined
		style="margin: 10px;"
	>
		<v-list-item three-line>
			<v-list-item-content style="display: block;">
				<v-btn color="blue-grey" class="ma-2 white--text">MySQL</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">MS-SQL</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">PostgreSQL</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">MongoDB</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">GraphQL</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">Firebase Store</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">Google Cloud Database</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">AWS RDS</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">AWS Redshift</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">AWS DynamoDB</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">SQL query</v-btn>
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