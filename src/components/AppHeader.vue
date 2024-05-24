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
	<header class="bg-white">
		<div class="my_box_container">
			<div class="row align-items-center">
				<div
					class="col-12 col-md-2 text-center text-md-start mb-3 mb-md-0 p-0"
				>
					<img :src="getImg(logoHeader)" alt="" />
				</div>
				<div
					class="col-12 col-md-10 p-0 gap-3 d-flex justify-content-end"
				>
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
	padding: 2rem 0;
	border-bottom: 2px solid white;
}

a:hover {
	border-bottom: 2px solid blue;
	box-sizing: border-box;
}
</style>
