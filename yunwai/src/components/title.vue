<template>
  <h3 v-html="text"></h3>
</template>

<script>
export default {
	props: ['text'],
	data () {
		return {}
	}
}
</script>

<style lang="scss" scoped>
h3 {
	padding-left: .08rem;
	font-size: .18rem;
  font-weight: bold;
	line-height: .25rem;
	position: relative;
	&::before {
		content: "";
		position: absolute;
		left: 0;
		top: .02rem;
		width: .04rem;
		height: .2rem;
		background: #EFB336;
	}
}
</style>
