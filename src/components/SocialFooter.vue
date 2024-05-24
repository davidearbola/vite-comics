<script>
export default {
	name: "SocialFooter",
	data() {
		return {
			socialIcon: [
				"footer-facebook.png",
				"footer-periscope.png",
				"footer-pinterest.png",
				"footer-twitter.png",
				"footer-youtube.png",
			],
		};
	},
	methods: {
		getImg(path) {
			let risultato = new URL("../assets/img/" + path, import.meta.url);
			return risultato.href;
		},
	},
};
</script>

<template>
	<div class="box_social">
		<div class="my_box_container">
			<div class="row align-items-center justify-content-between">
				<div class="col-2">
					<div class="my_border">SIGN UP NOW!</div>
				</div>
				<div class="col-6">
					<div class="row align-items-center justify-content-between">
						<div class="col-5 text-end">
							<h5 class="follow_text m-0">FOLLOW US</h5>
						</div>
						<div class="col-7 d-flex gap-4">
							<img
								v-for="img in socialIcon"
								:src="getImg(img)"
								alt=""
							/>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<style scoped>
.box_social {
	background-color: #303030;
	padding: 2rem;
}

.my_border {
	padding: 1rem;
	border: 2px solid blue;
	color: white;
}

.follow_text {
	color: blue;
}

img {
	height: 2rem;
}
</style>
