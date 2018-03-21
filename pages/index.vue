<template>
	<section class="container">
		<h1 class="h1">Jesse Breneman</h1>
		<h2 class="h2">Front-end web developer, Vue aficionado, tea fiend, robot...</h2>
		<h3 class="h3">Links to my stuff</h3>

		<ul class="linklist">
			<li class="link-item" v-for="item in linkItems" :key="item.name">
				<a :href="item.url" class="link">{{ item.name }}</a>
			</li>
		</ul>

	</section>
</template>

<script>
export default {
  data() {
	return {
		linkItems: [
			{
				name: 'Github',
				url: 'https://github.com/jbreneman'
			},
			{
				name: 'suggestmycolors',
				url: 'http://projects.jessebreneman.com/suggest/'
			},
			{
				name: 'background gradient builder',
				url: 'https://background-gradient-builder.netlify.com/'
			},
			{
				name: '(tea)timer (a PWA)',
				url: 'https://teatimer.website/'
			},
			{
				name: 'lazuli.js',
				url: 'https://www.npmjs.com/package/@jbreneman/lazuli-js'
			}
		]
	};
  }
}
</script>


<style scoped>
.container {
	width: 100%;
	height: 100%;
	max-width: 800px;
	margin: auto;
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	mix-blend-mode: overlay;
}

.h1 {
	color: white;
	font-size: 4rem;
	margin-bottom: .5rem;
	text-align: center;
}

.h2 {
	color: white;
	font-size: 1.5rem;
	margin-bottom: 4rem;
	text-align: center;
}

.h3 {
	color: white;
	font-size: 1.25rem;
	text-align: center;
	margin-bottom: 2rem;
}

.linklist {
	display: flex;
	flex-wrap: wrap;
	justify-content: center;
	list-style-type: none;
	padding: 0;
}

.link-item {
	display: flex;
	margin-bottom: 1rem;
}

.link {
	mix-blend-mode: overlay;
	background-color: white;
	color: rgba(0, 0, 0, .75);
	padding: .5rem;
	margin: 0 .5rem;
	text-decoration: none;
	border-radius: 1px;
}

.link:hover {
	color: white;
	background-color: rgba(0, 0, 0, .75);
}
</style>
