<script>
	import logo from '$lib/images/svelte-logo.svg';
	import github from '$lib/images/github.svg';
	import ArrowRight from '$lib/components/ArrowRight.svelte';
	import { page } from '$app/stores';
</script>


<sidebar>
	<div class="text-right w-80 p-10">
		{#if $page.url.pathname!="/about" && $page.url.pathname!="/resume"}
		<a href="/">
			<div class="text-3xl color" style="color:rgb(188, 188, 188); line-height:2; font-size:2.2em; text-decoration:inherit;">mathew d</div></a>
			{#if $page.url.pathname=="/"}
		<div>I'm an artist and designer.</div>
		<a href="/about">
			<div style="color:#858585; text-decoration:inherit;">more<ArrowRight />
		</div></a>
		{/if}
		{/if}
	</div>
</sidebar>
<style>
</style>
