<template>
	<div>
	  <v-card
	    class=""
	    max-width="100%"
	    style="margin: 10px;">
	    <v-card-text>
	      <div>2015.03 — 2017.02</div>
	      <p class="display-1 text--primary">
	        clickTRUE Pte Ltd
	      </p>
	      <p>Full Stack Developer</p>
	    </v-card-text>
	    <v-card-actions style="margin-top: -30px;">
	      <v-btn
	        text
	        color="teal accent-4"
	        @click="reveal1 = true"
	      >
	        Learn More
	      </v-btn>
	    </v-card-actions>

	    <v-expand-transition>
	      <v-card
	        v-if="reveal1"
	        class="transition-fast-in-fast-out v-card--reveal"
	        style="height: 100%;"
	      >
	        <v-card-text class="pb-0">
	          <p class="">
	            In the clickTRUE , I worked as a full stack developer to build web and mobile apps that are helpful for adv system. I worked in this company for several years. Working in clickTRUE, I majored Website and Mobile application development for startup companies and supported them to grow up based on internet infrastructure.
	          </p>
	        </v-card-text>
	        <v-card-actions class="pt-0">
	          <v-btn
	            text
	            color="teal accent-4"
	            @click="reveal1 = false"
	          >
	            Close
	          </v-btn>
	        </v-card-actions>
	      </v-card>
	    </v-expand-transition>
	  </v-card>

	  <v-card
	    class=""
	    max-width="100%"
	    style="margin: 10px;">
	    <v-card-text>
	      <div>2017.06 — 2018.05</div>
	      <p class="display-1 text--primary">
	        Concept Health
	      </p>
	      <p>Senior Back-End Engineer</p>
	    </v-card-text>
	    <v-card-actions style="margin-top: -30px;">
	      <v-btn
	        text
	        color="teal accent-4"
	        @click="reveal2 = true"
	      >
	        Learn More
	      </v-btn>
	    </v-card-actions>

	    <v-expand-transition>
	      <v-card
	        v-if="reveal2"
	        class="transition-fast-in-fast-out v-card--reveal"
	        style="height: 100%;"
	      >
	        <v-card-text class="pb-0">
	          <p class="">
	            Concept Health combines the power of Virtual Reality, IOT Sensors, and Artificial Intelligence to deliver healthcare services 24/7. Concept Health augment the ability of Community services provider to deliver services that are safe, cost effective and available 24/7 using our proprietary concepts and technology. I have built Ruby on Rails web server, Real time communication websocket, Restful API endpoints, and Unittest and I have managed Devops with CI/CD.
	          </p>
	        </v-card-text>
	        <v-card-actions class="pt-0">
	          <v-btn
	            text
	            color="teal accent-4"
	            @click="reveal2 = false"
	          >
	            Close
	          </v-btn>
	        </v-card-actions>
	      </v-card>
	    </v-expand-transition>
	  </v-card>

	  <v-card
	    class=""
	    max-width="100%"
	    style="margin: 10px;">
	    <v-card-text>
	      <div>2018.04 — Present</div>
	      <p class="display-1 text--primary">
	        Easy-Level
	      </p>
	      <p>Professional Blockchain and Web developer</p>
	    </v-card-text>
	    <v-card-actions style="margin-top: -30px;">
	      <v-btn
	        text
	        color="teal accent-4"
	        @click="reveal3 = true"
	      >
	        Learn More
	      </v-btn>
	    </v-card-actions>

	    <v-expand-transition>
	      <v-card
	        v-if="reveal3"
	        class="transition-fast-in-fast-out v-card--reveal"
	        style="height: 100%;"
	      >
	        <v-card-text class="pb-0">
	          <p class="">
	            EasyLevel works on 16 Advertising platforms, and gets its profits from the spread generated between Publisher and Advertiser, and from all views and clicks performed by visitors:
							Profits division table:
							[10% to the clickers]&nbsp;
							[10% to the Publisher]&nbsp;
							[80% to the Smart Contract which benefit goes to all EL users.]&nbsp;
							Easy-Level is Cryptocurrency based-world first decentralized P2P advertising platform. I've worked as a lead developer in Easy-level and managed team, project, devops, Blockchain integration, front-end, back-end development
	          </p>
	        </v-card-text>
	        <v-card-actions class="pt-0">
	          <v-btn
	            text
	            color="teal accent-4"
	            @click="reveal3 = false"
	          >
	            Close
	          </v-btn>
	        </v-card-actions>
	      </v-card>
	    </v-expand-transition>
	  </v-card>

	  <v-card
	    class=""
	    max-width="100%"
	    style="margin: 10px;">
	    <v-card-text>
	      <div>2019.07 — Present</div>
	      <p class="display-1 text--primary">
	        Geomiq
	      </p>
	      <p>Senior Backend Developer</p>
	    </v-card-text>
	    <v-card-actions style="margin-top: -30px;">
	      <v-btn
	        text
	        color="teal accent-4"
	        @click="reveal4 = true"
	      >
	        Learn More
	      </v-btn>
	    </v-card-actions>

	    <v-expand-transition>
	      <v-card
	        v-if="reveal4"
	        class="transition-fast-in-fast-out v-card--reveal"
	        style="height: 100%;"
	      >
	        <v-card-text class="pb-0">
	          <p class="">
	            GEOMIQ is a Data-Driven manufacturing company focusing in 3D printing. There is a web platform that users can upload CAD files to get quotation or delivered products of 3D objects. I'd contracted as a full time remote developer and worked in Backend mostly to implement 3D related tasks and SEO.
	          </p>
	        </v-card-text>
	        <v-card-actions class="pt-0">
	          <v-btn
	            text
	            color="teal accent-4"
	            @click="reveal4 = false"
	          >
	            Close
	          </v-btn>
	        </v-card-actions>
	      </v-card>
	    </v-expand-transition>
	  </v-card>
	</div>
</template>

<script>
  export default {
    data: () => ({
      reveal1: false,
      reveal2: false,
      reveal3: false,
      reveal4: false,
    }),
  }
</script>

<style>
.v-card--reveal {
  bottom: 0;
  opacity: 1 !important;
  position: absolute;
  width: 100%;
}

.v-application .teal--text.text--accent-4 {
	color: green!important;
}
</style>