<template>
	<div id="app">
		<NavigationBar />
		<FadeTranslateTransition mode="out-in" duration="0.4s">
			<router-view/>
		</FadeTranslateTransition>
	</div>
</template>

<style lang="scss">
@import 'assets/main.scss';

.page {
	width: 100%;
	min-height: 92vh;
	margin-top: 8vh;
	display: flex;
	justify-content: center;
	text-align: center;
}
</style>

<script>
import NavigationBar from '@/components/NavigationBar.vue'
import FadeTranslateTransition from '@/components/FadeTranslateTransition.vue'

export default {
	components: {
		NavigationBar,
		FadeTranslateTransition
	}
}
</script>
