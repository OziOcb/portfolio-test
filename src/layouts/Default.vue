<template>
	<div class="layout">
		<header class="header">
			<div class="header__inner container">
				<strong>
					<g-link to="/">{{ $static.metadata.siteName }}</g-link>
				</strong>
				<nav class="nav">
					<g-link class="nav__link" to="/">Home</g-link>
					<g-link class="nav__link" to="/about/">About</g-link>
				</nav>
			</div>
		</header>
		<slot />
	</div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style lang="scss">
body {
	margin: 0;
	padding: 0;
	font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
	line-height: 1.5;
}

.header {
	position: fixed;
	top: 0;
	right: 0;
	left: 0;
	background-color: #fff;

	&__inner {
		margin-bottom: 20px;
		display: flex;
		height: 80px;
		justify-content: space-between;
		align-items: center;
	}
}

.nav__link {
	margin-left: 20px;
}
</style>
