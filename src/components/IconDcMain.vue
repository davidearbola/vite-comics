<script>
export default {
	name: "IconDcMain",
	data() {
		return {
			iconsDc: [
				{
					name: "DIGITAL COMICS",
					icon: "./src/assets/img/buy-comics-digital-comics.png",
				},
				{
					name: "DC MERCHANDISE",
					icon: "./src/assets/img/buy-comics-merchandise.png",
				},
				{
					name: "SUBSCRIPTION",
					icon: "./src/assets/img/buy-comics-subscriptions.png",
				},
				{
					name: "COMIC SHOP LOCATOR",
					icon: "./src/assets/img/buy-comics-shop-locator.png",
				},
				{
					name: "DC POWER VISA",
					icon: "./src/assets/img/buy-dc-power-visa.svg",
				},
			],
		};
	},
};
</script>

<template>
	<div class="my_bg_blue text-white">
		<div class="row my_box_container justify-content-between">
			<div
				v-for="iconElement in iconsDc"
				class="col-auto py-3 d-flex align-items-center gap-2"
			>
				<img :src="iconElement.icon" />
				<span>{{ iconElement.name }}</span>
			</div>
		</div>
	</div>
</template>

<style scoped>
img {
	height: 2rem;
}
</style>
