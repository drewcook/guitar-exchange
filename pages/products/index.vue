<template>
	<div class="container">
		<h1>Products</h1>
    <LargeCardDisplay :cardsSection="largeCardInfo[0]" />
		<SmallCardDisplay
			v-for="cardInfo in smallCardInfo"
			:key="cardInfo.id"
			:cardsSection="cardInfo"
		/>
	</div>
</template>

<script>
	import { largeCardSections, smallCardSections } from '@/assets/data'
	export default {
		data() {
			return {
				largeCardInfo: largeCardSections,
				smallCardInfo: smallCardSections,
			}
		},
	}
</script>

<style></style>
