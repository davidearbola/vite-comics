<script>
export default {
	name: "AppHeader",
	data() {
		return {
			logoHeader: "dc-logo.png",
			linkMenu: [
				"CHARACTERS",
				"COMICS",
				"MOVIES",
				"TV",
				"GAMES",
				"COLLECTIBLES",
				"VIDEOS",
				"FANS",
				"NEWS",
				"SHOP",
			],
		};
	},
	methods: {
		getImg(path) {
			let risultato = new URL(`../assets/img/${path}`, import.meta.url);
			return risultato.href;
		},
	},
};
</script>

<template>
	<header class="bg-white p-3">
		<div class="my_box_container">
			<div class="row align-items-center">
				<div
					class="col-12 col-md-2 text-center text-md-start mb-3 mb-md-0 p-0"
				>
					<img :src="getImg(logoHeader)" alt="" />
				</div>
				<div class="col-12 col-md-10 p-0 d-flex justify-content-around">
					<a v-for="link in linkMenu" href="#">{{ link }}</a>
				</div>
			</div>
		</div>
	</header>
</template>

<style scoped>
img {
	width: 3rem;
}

a {
	font-size: 14px;
	text-decoration: none;
	color: black;
}
</style>
