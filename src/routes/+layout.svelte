<script>
	import Header from '$lib/components/Header.svelte';
	import Sidebar from '$lib/components/Sidebar.svelte';
	import './styles.css';
	import '../app.css';

	import { page } from '$app/stores';
</script>

<div class="app">
	<Header />
	<div class="flex">
		<div class="lg:hidden">
			{#if $page.url.pathname=="/"}
			<a href="/about"><div class="fixed left-5 top-7 z-50 w-6 h-6"><img src="/logo.png" class="w-6" /></div></a>
			{:else}
			<a href="/"><div class="fixed left-5 top-7 z-50 w-6 h-6"><img src="/logo.png" class="w-6" /></div></a>
			{/if}
		</div>
		<div class="hidden lg:flex lg:flex-none h-14">
			<Sidebar />
		</div>
		<div class="grow h-14">
	<main>
		<slot />
		<!-- <h1 class="text-3xl font-bold underline">
			Hello world!
		  </h1> -->
	</main>
</div>
</div>

	<footer>
		<!-- <p>visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to learn SvelteKit</p> -->
		<!-- Hotjar Tracking Code for mathew d -->
<script>
    (function(h,o,t,j,a,r){
        h.hj=h.hj||function(){(h.hj.q=h.hj.q||[]).push(arguments)};
        h._hjSettings={hjid:3341555,hjsv:6};
        a=o.getElementsByTagName('head')[0];
        r=o.createElement('script');r.async=1;
        r.src=t+h._hjSettings.hjid+j+h._hjSettings.hjsv;
        a.appendChild(r);
    })(window,document,'https://static.hotjar.com/c/hotjar-','.js?sv=');
</script>
	</footer>
</div>
