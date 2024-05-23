<script>
export default {
	data() {
		return {
			linkFooter: [
				{
					titolo: "DC COMICS",
					link: [
						"Characters",
						"Comics",
						"Movies",
						"TV",
						"Games",
						"Videos",
						"News",
					],
				},
				{
					titolo: "SHOP",
					link: ["Shop DC", "Shop DC Collectibles"],
				},
				{
					titolo: "DC",
					link: [
						"Terms Of Use",
						"Privacy policy (New)",
						"Ad Choices",
						"Advertising",
						"Jobs",
						"Subscriptions",
						"Talent Workshops",
						"CPSC Certificates",
						"Ratings",
						"Shop Help",
						"Coontact Us",
					],
				},
				{
					titolo: "SITES",
					link: [
						"DC",
						"MAD Magazine",
						"DC Kids",
						"DC Universe",
						"DC Power Visa",
					],
				},
			],
		};
	},
};
</script>

<template>
	<div class="box_link p-3">
		<div class="my_box_container">
			<div class="row">
				<div class="col-6">
					<div class="row">
						<div class="col-4 d-flex flex-column gap-3">
							<div class="d-flex flex-column">
								<h3>{{ linkFooter[0].titolo }}</h3>
								<a
									v-for="link in linkFooter[0].link"
									href="#"
									>{{ link }}</a
								>
							</div>
							<div class="d-flex flex-column">
								<h3>{{ linkFooter[1].titolo }}</h3>
								<a v-for="link in linkFooter[1].link" href="">{{
									link
								}}</a>
							</div>
						</div>
						<div class="col-4">
							<div class="d-flex flex-column">
								<h3>{{ linkFooter[2].titolo }}</h3>
								<a v-for="link in linkFooter[2].link" href="">{{
									link
								}}</a>
							</div>
						</div>
						<div class="col-4">
							<div class="d-flex flex-column">
								<h3>{{ linkFooter[3].titolo }}</h3>
								<a v-for="link in linkFooter[3].link" href="">{{
									link
								}}</a>
							</div>
						</div>
					</div>
				</div>
				<div class="logo_box col-6"></div>
			</div>
		</div>
	</div>
</template>

<style scoped>
.box_link {
	background-image: url(../assets/img/footer-bg.jpg);
	color: lightgray;
}

.logo_box {
	background-image: url(../assets/img/dc-logo-bg.png);
	background-size: contain;
	background-repeat: no-repeat;
	background-position: center;
}

h3 {
	font-size: 18px;
	color: white;
}

a {
	text-decoration: none;
	color: lightgray;
	font-size: 12px;
}
</style>
