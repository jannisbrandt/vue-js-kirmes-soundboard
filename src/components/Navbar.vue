<template>
	<nav>
		<v-toolbar app dark>
			<!-- <v-toolbar-side-icon v-on:click="isDrawerOpen = !isDrawerOpen" /> -->
			<v-toolbar-title class="text-sm-center ma-auto">
        🎤 <span class="font-weight-black"> KIRMES SOUNDBOARD </span> <span class="font-weight-light">APP</span> 🎉
      </v-toolbar-title>
		</v-toolbar>
<!--
		<v-navigation-drawer dark app v-model="isDrawerOpen">
			<v-list>
				<v-list-tile v-on:click="navigate('/')">
					<v-list-tile-action>
						<v-icon>headset</v-icon>
					</v-list-tile-action>
					<v-list-tile-content>
						<v-list-tile-title>Soundboard</v-list-tile-title>
					</v-list-tile-content>
				</v-list-tile>

				<v-list-tile v-on:click="navigate('about')">
					<v-list-tile-action>
						<v-icon>info</v-icon>
					</v-list-tile-action>
					<v-list-tile-content>
						<v-list-tile-title>About</v-list-tile-title>
					</v-list-tile-content>
				</v-list-tile>
			</v-list>
		</v-navigation-drawer>

		-->

	</nav>
</template>

<script>
export default {
	name: 'Navbar',
	data () {
		return {
			isDrawerOpen: false
		}
	},
	methods: {
		navigate: function (route) {
			this.$router.push(route);
		}
	}
}
</script>

