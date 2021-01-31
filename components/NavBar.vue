<template>
	<nav class="navbar" role="navigation" aria-label="main navigation">
		<div class="navbar-left">
			<div class="navbar-brand">
				<nuxt-link to="/" class="nav-item">
					<img src="/images/logo.png" alt="Web School logo" class="logo">
				</nuxt-link>	
			</div>
			<div class="navbar-menu">
				<nuxt-link to="/" class="nav-item">Home</nuxt-link>
				<nuxt-link to="/" class="nav-item">Technologies</nuxt-link>
				<nuxt-link to="/" class="nav-item">Blogs</nuxt-link>
			</div>
		</div>
		<div class="navbar-right">
			<nuxt-link to="/" class="nav-item">Quick Search</nuxt-link>
			<nuxt-link to="/" class="nav-item">About</nuxt-link>
		</div>
	</nav>
</template>
<style lang="stylus" scoped>
	.navbar
		display: flex
		align-items: center
		justify-content: space-between
		padding: 10px
		background-color: #3bb78f;
		background-image: linear-gradient(315deg, #3bb78f 0%, #0bab64 74%);
		box-shadow: 0px 15px 10px -15px rgba(0,0,0,0.1)
		.navbar-left
			display: inherit
			align-items: inherit
			.navbar-brand
				.logo
					width: 80px
		.nav-item
			font-family: 'p-regular'
			font-size: 16px
			color: white
			padding: 0 5px
</style>