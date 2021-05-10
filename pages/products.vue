<template>
	<div class="container">
		<h1>Products</h1>
		<SmallCardDisplay
			v-for="cardInfo in smallCardInfo"
			:key="cardInfo.id"
			:cardsSection="cardInfo"
		/>
	</div>
</template>

<script>
	import { smallCardSections } from '@/assets/data'
	export default {
		data() {
			return {
				smallCardInfo: smallCardSections,
			}
		},
	}
</script>

<style></style>
