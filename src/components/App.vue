<template>
  <div id="app">
    Cute animals!
	<div>
		<cute-animal v-for="url in urlList" v-bind:url="url" v-bind:key="url" />
	</div>


  </div>
</template>

<script>
import CuteAnimal from './CuteAnimal.vue';

export default {
	name: 'app',
	components: {
		'cute-animal': CuteAnimal
	},
	data: function() {
		return {
			urlList: [
				'https://i.ytimg.com/vi/J0EUxEkm4kc/maxresdefault.jpg',
				'https://i.pinimg.com/736x/78/b8/a5/78b8a51098ef44932f2c459e23861b61.jpg',
				'https://i.ytimg.com/vi/M9fv8aFhyXU/maxresdefault.jpg',
				'https://img.buzzfeed.com/buzzfeed-static/static/2014-11/5/13/enhanced/webdr07/enhanced-5913-1415212088-2.jpg?downsize=715:*&output-format=auto&output-quality=auto'
			]
		};
	}
}
</script>

<!-- CSS libraries -->
<style src="normalize.css/normalize.css"></style>

<!-- Global CSS -->
<style>
  code {
    font-family: Menlo, Monaco, Lucida Console, Liberation Mono, DejaVu Sans Mono, Bitstream Vera Sans Mono, Courier New, monospace, serif;
    font-size: 0.9em;
    white-space: pre-wrap;
    color: #2c3e50;
  }

  code::before, code::after {
    content: '`';
  }
</style>

<!-- Scoped component css -->
<!-- It only affect current component -->
<style scoped>
  #app {
    text-align: center;
  }

  #app h1 {
    color: #2c3e50;
    font-weight: 300;
    margin: 0;
  }
  div {
	  background-color: hotpink;
  }
</style>
