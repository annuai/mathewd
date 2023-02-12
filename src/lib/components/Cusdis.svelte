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
     appId: "b9e510b6-80d9-4d40-b519-e1fbde56524f",
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