<template>
  <v-card
    class=""
    max-width="635"
    outlined
    style="margin: 10px;"
  >
    <v-list-item three-line>
      <v-list-item-content>
        <div class="overline mb-4">
          Dates attended or expected graduation : 2009 – 2014
        </div>
        <v-list-item-title class="headline mb-1">
          Don Mariano Marcos Memorial State University
        </v-list-item-title>
        <v-list-item-subtitle>
        	Degree Name : Bachelor's degreeField Of StudyEngineering
				</v-list-item-subtitle>
      </v-list-item-content>

      <v-list-item-avatar
        tile
        size="80"
        color="grey"
      >
      	<img src="/university.png" />
      </v-list-item-avatar>
    </v-list-item>

    <v-card-actions>
      <v-btn
        outlined
        rounded
        text
        v-on:click="learnmore"
        style="color: green;border: 0px;"
      >
        Learn more
      </v-btn>
    </v-card-actions>
  </v-card>
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