<template>
	<div>
	  <v-card
	    class=""
	    max-width="100%"
	    outlined
	    style="margin: 10px;"
	  >
	    <v-list-item three-line>
	      <v-list-item-content>
	      	<img src="/cert1.png" style="width: 100%" />
	      </v-list-item-content>
	    </v-list-item>
	  </v-card>

	  <v-card
	    class=""
	    max-width="100%"
	    outlined
	    style="margin: 10px;"
	  >
	    <v-list-item three-line>
	      <v-list-item-content>
	      	<img src="/cert2.png" style="width: 100%" />
	      </v-list-item-content>
	    </v-list-item>
	  </v-card>
	</div>
</template>

<script>
  export default {
    data: () => ({
    }),
    methods: {
    	learnmore: function() {
    		window.open('https://www.linkedin.com/school/don-mariano-marcos-memorial-state-university/', '_blank');
    	}
    }
  }
</script>

<style scoped>
</style>