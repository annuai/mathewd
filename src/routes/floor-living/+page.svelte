<script>
	import { Splide, SplideSlide } from '@splidejs/svelte-splide';
	import '@splidejs/svelte-splide/css';
	
	import BackHome from '$lib/components/BackHome.svelte'

	import { page } from '$app/stores';
	import Cusdis from '$lib/components/Cusdis.svelte'
	// import Cusdis from "$lib/components/svelte-cusdis";
</script>
<svelte:head>
	<title>floor living - mathew d</title>
	<meta name="description" content="floor living - mathew d" />
</svelte:head>
<div>
<div>
<div style="padding:56.25% 0 0 0;position:relative;">
<iframe src="https://player.vimeo.com/video/254954384?h=5a6eadae63" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen="" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="floor living" class=""></iframe>
</div>
</div>
<br>
<div class="px-3 lg:px-0">
		<h2>floor living</h2><br>
    <div class="text-content max-w-screen-sm">
<small>the practice of floor living is the idea of involving the floor in more daily activities without it being merely a surface to stand, walk and place furniture on. this way of living has been present in several eastern, african and middle eastern cultures for millennia, until the recent wave of modernisation. the increasing epidemic of back aches and related health issues can be connected to the proliferation and excessive dependence and misuse of furniture. with this project, I attempt to bring back the floor with objects that are designed to accommodate a wide variety of sitting postures from the erect seiza position to the meditative lotus position, to the basic squat. the rugs and cushions are to be integrated into daily practice with other supporting furniture such as short tables for working or eating. <br>
<br>the most simple advantage of working while sitting on the floor can be summarised with one practical example: when one is sitting on the floor, there is the constant need to move and possible erect oneself to reach things, such as to find a pen, or reach for a bookshelf - this constant, low intensity exercise that is spread throughout the daily routine is the key to long and healthy life, as opposed to brief bursts of intense workouts at a gym. the act of eating on the floor also engages the abdominal muscles into a constant back and forth movement while reaching for the food - this aids in the efficiency of the digestion process.<br>

</small>
<br>
</div>
</div>
</div>

<div> 
<br>
<Splide aria-label="My Favorite Images" options={ {
	rewind: true,
	rewindSpeed:1,
	autoplay: true,
	interval: 3000,
	pagination: false,
  } }>
	<SplideSlide>
		<img src="images/floor-living/1.jpg" class="w-full" alt="Image 1"/>
		<div class="text-center gallery-caption mx-0">initial models for the pieces.</div>
	</SplideSlide>
	<SplideSlide>
		<img src="images/floor-living/2.gif" class="w-full" alt="Image 2"/>
		<div class="text-center gallery-caption mx-0">postures were studied and then photographed to make the graphics for the pieces. this is the lotus position.</div>
	</SplideSlide>
	<SplideSlide>
		<img src="images/floor-living/3.jpg" class="w-full" alt="Image 3"/>
		<div class="text-center gallery-caption mx-0">screen printing color options</div>
	</SplideSlide>
	<SplideSlide>
		<img src="images/floor-living/4.jpg" class="w-full" alt="Image 4"/>
		<div class="text-center gallery-caption mx-0">a few people were invited to be observed on how they take to sitting on the floor. these were people from all age groups above 20 years. they were asked to sit for an hour.</div>
	</SplideSlide>
</Splide>
<br>
<Cusdis pageId ="floor-living" pageTitle="floor living" />
<!-- <script async defer src="http://localhost:5173/cusdis.es.js"></script>
<div id="cusdis_thread"
  data-host="https://cusdis.com"
  data-app-id="b9e510b6-80d9-4d40-b519-e1fbde56524f"
  data-page-id="floor-living"
  data-page-url="floor-living"
  data-page-title="floor living"
></div> -->
<!-- <Cusdis
 attrs = {{
     appId: "b9e510b6-80d9-4d40-b519-e1fbde56524f",
     pageId: "floor-living",
     pageUrl: "https://mathewd.com/",
     pageTitle: "floor living",
	 theme: "light"
 }}
/> -->
<br>
<BackHome />
<br>
 <br>
</div>