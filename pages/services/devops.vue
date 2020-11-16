<template>
	<v-card
		class=""
		max-width="100%"
		outlined
		style="margin: 10px;"
	>
		<v-list-item three-line>
			<v-list-item-content style="display: block;">
				<v-btn color="blue-grey" class="ma-2 white--text">Github</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">Gitlab</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">CI/CD</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">Docker</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">Docker-compose</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">Kubernates</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">Google Cloud Platform</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">AWS EC2</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">AWS Elastic Beanstalk</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">AWS ECS/ECR/EKS</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">AWS Load Balancing</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">AWS Route53</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">AWS IAM</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">AWS Certificate Manager</v-btn>
				<v-btn color="blue-grey" class="ma-2 white--text">Microsoft Azure</v-btn>
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