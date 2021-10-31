<template>
	<v-container fluid grid-list-lg>
		<v-layout wrap>
			<v-flex xs6 md3 v-for="(sound, index) in sounds" :key="index">
				<v-card v-on:click="play(sound.sound)">
					<v-card-text>
						<v-icon color="pink" class="button--play" x-large>play_circle</v-icon>
						<p>{{ sound.title }}</p>
					</v-card-text>
				</v-card>
			</v-flex>
		</v-layout>
	</v-container>
</template>

<style>
.v-card:hover {
  background-color: #f0a6bf;
}
</style>

<script>
export default {
	name: 'Sounds',
	data () {
		return {
			sounds: [
				{
					title: "Ready",
					sound: "ready.mp3"
				},
				{
					title: "Horn",
					sound: "horn.mp3"
				},
				{
					title: "Achtung",
					sound: "achtung_fertig_los.mp3"
				},
				{
					title: "Action",
					sound: "action-power-los.mp3"
				},
				{
					title: "Jetzt geht's los",
					sound: "jetzt_gehts_los.mp3"
				},
				{
					title: "Yalla Habibi",
					sound: "yalla_habibi.mp3"
				},
				{
					title: "80 Meter",
					sound: "80meter.mp3"
				},
        {
          title: "Around the World",
          sound: "around-the-world.mp3"
        },
        {
          title: "Here we go",
          sound: "here-we-go.mp3"
        },
        {
          title: "Mädels",
          sound: "maedels.mp3"
        },
        {
          title: "Hey Hallöchen",
          sound: "hey-haellochen.mp3"
        },
        {
          title: "Hashtag",
          sound: "hashtag.mp3"
        },
        {
          title: "Alles geben",
          sound: "allesgeben.mp3"
        },
        {
          title: "Kreuz & Quer",
          sound: "kreuz-und-quer.mp3"
        },
        {
          title: "Kindergeburtstag",
          sound: "kindergeburtstag.mp3"
        },
        {
          title: "Jetzt erst Recht",
          sound: "jetzt-erst-recht.mp3"
        },
        {
          title: "Kopf in Nacken",
          sound: "kopf-in-nacken.mp3"
        },
        {
          title: "Fühl dich Funky",
          sound: "fuehl-dich-funky.mp3"
        }
        ,
        {
          title: "Jetzt geht's los",
          sound: "jetzt-gehts-los.mp3"
        }
        ,
        {
          title: "uuuuuund Los",
          sound: "uuuuund-los.mp3"
        }
        ,
        {
          title: "Abgehts",
          sound: "abgehts.mp3"
        }
        ,
        {
          title: "Super",
          sound: "super.mp3"
        }
			]
		}
	},
	methods: {
		play: function (name) {
			let audio = new Audio(require('@/assets/sounds/' + name));
			audio.play();
		}
	}
}
</script>

