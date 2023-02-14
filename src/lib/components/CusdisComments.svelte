<script>
    import { page } from '$app/stores';
    import Cusdis from "$lib/components/svelte-cusdis";
    export let pageId;
    export let pageTitle;
</script>
<br>
<br>
<hr>
<br>
<br>
<div class="px-3 lg:pl-0 lg:pr-5">
<div class="px-3 pl-4 lg:pl-1 text-xl font-bold">comments</div>
<br>
<div class="px-3 lg:pl-0 lg:pr-5">
<Cusdis
 attrs = {{
     appId: "b9a15486-27e3-41a1-b5c3-1410d5ff4348",
     pageId: pageId,
     pageUrl: "https://mathewd.com/"+$page.url.pathname+"",
     pageTitle: pageTitle,
	 theme: "light"
 }}
/>
</div>
</div>
<br>
<hr>