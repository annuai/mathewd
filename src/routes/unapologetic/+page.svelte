<script>
	import { Splide, SplideSlide } from '@splidejs/svelte-splide';
	import '@splidejs/svelte-splide/css';

	import Image from '$lib/components/Image.svelte'
	import BackHome from '$lib/components/BackHome.svelte'
</script>
<svelte:head>
	<title>unapologetic automatic - mathew d</title>
	<meta name="description" content="unapologetic automatic - mathew d" />
</svelte:head>
<div>
	<div>
		<Image src="images/unapologetic/DSC00317.jpg" alt="unapologetic" />
	</div>
	</div>
	
	<div class="px-3 lg:px-0">
		<br>
	<div><small><h2>unapologetic automatic</h2><br><div class="text-content">
	this is my first collection of poetry. 50 handbound copies were made.
	
	</div></small><br>
	</div></div>


	<Splide aria-label="My Favorite Images" options={ {
		rewind: true,
		rewindSpeed:1,
		autoplay: true,
		interval: 3000,
	  } }>
		<SplideSlide>
			<img src="images/unapologetic/DSC00346.jpg" class="w-full" alt="Image 1"/>
		</SplideSlide>
		<SplideSlide>
			<img src="images/unapologetic/DSC00344.jpg" class="w-full" alt="Image 1"/>
		</SplideSlide>
		<SplideSlide>
			<img src="images/unapologetic/DSC00338.jpg" class="w-full" alt="Image 1"/>
		</SplideSlide>
		<SplideSlide>
			<img src="images/unapologetic/DSC00330.jpg" class="w-full" alt="Image 1"/>
		</SplideSlide>
	</Splide>
		
	<div class="image-gallery" gid="8">
	<!-- {image 27}
	{image 26}
	{image 25}
	{image 24} -->
	</div><br>
	<br>
	<br>
	<hr><br>
	<br>
	<BackHome />
	<br>