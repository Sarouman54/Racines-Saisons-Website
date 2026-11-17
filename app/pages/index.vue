<template>
	<section class="flex flex-col gap-4">
		<div class="flex w-full flex-col items-center px-gutter gap-4">
			<hgroup class="space-y-2">
				<h1>L'épicerie locale en<br />circuit-court</h1>
				<p class="text-center">Manger frais, de saison et français</p>
			</hgroup>

			<NuxtLink to="/produits" class="button-link px-14 text-center sm:w-auto md:px-32">Découvrir nos produits
			</NuxtLink>
		</div>

		<img src="/img/hero-800.avif"
			srcset="/img/hero-480.avif 480w, /img/hero-800.avif 800w, /img/hero-1280.avif 1280w"
			alt="Paniers de produits frais" class="aspect-4/5 w-full object-cover object-center md:aspect-auto" fetchpriority="high"/>
	</section>
</template>