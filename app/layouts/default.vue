<template>
	<header class="flex items-center gap-8 p-gutter">
		<NuxtLink to="/">
			<picture>
				<source media="(min-width: 48rem)" srcset="/logo-desktop.svg" width="200" height="40"/>
				<img src="/logo-mobile.svg" width="100" height="20" alt="Logo de Racines & Saisons, retour à l'accueil" />
			</picture>
		</NuxtLink>
		<AppNav />
	</header>
	<slot />
</template>