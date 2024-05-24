<script>
import LinkFooter from "./LinkFooter.vue";
import SocialFooter from "./SocialFooter.vue";

export default {
	name: "AppFooter",
	components: {
		LinkFooter,
		SocialFooter,
	},
};
</script>

<template>
	<footer>
		<LinkFooter />
		<SocialFooter />
	</footer>
</template>

<style scoped></style>
