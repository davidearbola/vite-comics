<script>
import ContentMain from "./ContentMain.vue";
import IconDcMain from "./IconDcMain.vue";

export default {
	name: "AppMain",
	components: {
		ContentMain,
		IconDcMain,
	},
};
</script>

<template>
	<main>
		<div class="jumbotron"></div>
		<ContentMain />
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
