<script setup lang="ts">
const links = [
	{ to: '/', label: 'Accueil', icon: resolveComponent('LucideHouse') },
	{ to: '/partenaires', label: 'Nos partenaires', icon: resolveComponent('LucideUsersRoundCollaboration') },
	{ to: '/produits', label: 'Nos produits', icon: resolveComponent('LucideGroceries') },
];
</script>

<template>
	<nav aria-label="Navigation principale" class="fixed inset-x-gutter bottom-gutter rounded-full bg-surface md:inset-x-0 md:bottom-auto md:top-0 md:rounded-none">
		<ul class="flex justify-center gap-4 md:justify-start">
			<li v-for="link in links" :key="link.to">
				<NuxtLink :to="link.to" class="group flex min-h-14 min-w-16 flex-col items-center justify-center font-semibold text-font-inactive aria-[current=page]:text-accent md:flex-row md:gap-1 ">
					<component :is="link.icon" class="size-5" aria-hidden="true" />
					<span class="border-b-2 border-transparent md:border-none group-aria-[current=page]:border-accent">
						{{link.label }}
					</span>
				</NuxtLink>
			</li>
		</ul>
	</nav>
</template>