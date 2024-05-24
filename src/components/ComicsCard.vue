<script>
export default {
	name: "ComicsCard",
	props: ["card"],
};
</script>
<template>
	<div class="col-6 col-md-4 col-lg-2 p-2">
		<div class="mb-3">
			<img :src="card.thumb" alt="" />
		</div>
		<div>
			<p class="mb-0">{{ card.series.toUpperCase() }}</p>
			<span>{{ card.type }}</span
			><br />
			<span>{{ card.price }}</span
			><br />
		</div>
	</div>
</template>
<style scoped>
img {
	width: 100%;
	aspect-ratio: 1;
	object-fit: cover;
	object-position: 0% 0%;
}

span {
	font-size: 12px;
}
</style>
