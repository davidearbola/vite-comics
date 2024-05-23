<script>
export default {
	data() {
		return {
			socialIcon: [
				"./src/assets/img/footer-facebook.png",
				"./src/assets/img/footer-periscope.png",
				"./src/assets/img/footer-pinterest.png",
				"./src/assets/img/footer-twitter.png",
				"./src/assets/img/footer-youtube.png",
			],
		};
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
							<img v-for="img in socialIcon" :src="img" alt="" />
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
