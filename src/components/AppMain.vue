<script>
import ComicCardMain from "./ComicCardMain.vue";
import IconDcMain from "./IconDcMain.vue";

export default {
	name: "AppMain",
	components: {
		ComicCardMain,
		IconDcMain,
	},
};
</script>

<template>
	<main>
		<div class="jumbotron"></div>
		<ComicCardMain />
		<IconDcMain />
	</main>
</template>

<style scoped>
.jumbotron {
	background-image: url("../assets/img/jumbotron.jpg");
	height: 30rem;
	background-position: top;
}
</style>
