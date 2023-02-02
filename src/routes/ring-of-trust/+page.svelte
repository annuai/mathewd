<script>
	import { Splide, SplideSlide } from '@splidejs/svelte-splide';
	import '@splidejs/svelte-splide/css';

	import BackHome from '$lib/components/BackHome.svelte'
</script>
<svelte:head>
	<title>ring of trust - mathew d</title>
	<meta name="description" content="ring of trust - mathew d" />
</svelte:head>
<div>
	<div>

<div style="padding:56.25% 0 0 0;position:relative;">
<iframe src="https://player.vimeo.com/video/790747257?h=a564197452&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen="" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="the ring of trust"></iframe>
</div>

</div>
</div>
<div>
	<div>
		<br>
    <div class="text-content max-w-screen-sm px-3 lg:px-0">
    <h2>the ring of trust</h2><br>
<small>working as an industrial designer in a young company that makes medical devices, I encountered a challenge : how do I make sure that all the products put out look like they are created by the same brand? in designer lingo: how do I create a consistent design language, even when all the products use a variety of manufacturing techniques which result in completely different surface finishes and textures?<br>
<br>
this was the reason why a unifying element of form or texture was diffciult to implement across the product range. some products have molded parts, some are 3D printed plastic and some are fully machined out of metal. this meant that applying a uniform fillet, curve, pattern or color was impossible.<br>
<br>
my idea was to create a separate element that can be integrated into the design of all the products. this element would be uniform wherever it is applied. the company, Remidio, creates imaging devices for ophthalmologists - in simple terms: cameras for eye doctors. lens design and optical innovation are core to the R&amp;D process. the circle is found everywhere in the parts - light travels in metal cylinders, and the lenses are circular. the part that comes in contact with the patient is a cricle. so the element is a circle, a metal ring that goes on the devices.<br>
<br>
the color was selected after finding the closest metal match to the brand pantone color,. I worked with several anodizing specialists to find the right shade, and to ensure color consistency across batches.<br>
<br>
then I set to redesign all the products to integrate the ring of trust into them.<br>
</small><br>
</div>
</div>
</div>



<!-- <div class="image-gallery" gid="28">
{image 9}
{image 7}
{image 6}
{image 8}
{image 10}
</div> -->
<Splide aria-label="My Favorite Images" options={ {
	rewind: true,
	rewindSpeed:1,
	autoplay: true,
	interval: 3000,
	pagination: false,
  } }>
	<SplideSlide>
		<img src="images/ring-of-trust/aim.png" class="w-full" alt="Image 1"/>
	</SplideSlide>
	<SplideSlide>
		<img src="images/ring-of-trust/fop.png" class="w-full" alt="Image 1"/>
	</SplideSlide>
	<SplideSlide>
		<img src="images/ring-of-trust/mrd.png" class="w-full" alt="Image 1"/>
	</SplideSlide>
	<SplideSlide>
		<img src="images/ring-of-trust/psl.png" class="w-full" alt="Image 1"/>
	</SplideSlide>
	<SplideSlide>
		<img src="images/ring-of-trust/vistaro.png" class="w-full" alt="Image 1"/>
	</SplideSlide>
</Splide>

<br>
<hr>
<br>
<br>
<BackHome />
<br>