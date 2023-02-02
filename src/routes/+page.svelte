<script type="ts">
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
	import { onMount,onDestroy } from "svelte"; 
	import jQuery from 'jquery';
	import { Splide, SplideSlide } from '@splidejs/svelte-splide';
	import '@splidejs/svelte-splide/css';

	import { fade } from 'svelte/transition';
	import { inview } from 'svelte-inview';

	import Image from '$lib/components/Image.svelte';
	import ArrowRight from '$lib/components/ArrowRight.svelte';

	import AOS from 'aos';
	import 'aos/dist/aos.css'; // You can also use <link> for styles


	onMount(() => {
		AOS.init({
			// Global settings:
			disable: false, // accepts following values: 'phone', 'tablet', 'mobile', boolean, expression or function
			startEvent: 'DOMContentLoaded', // name of the event dispatched on the document, that AOS should initialize on
			initClassName: 'aos-init', // class applied after initialization
			animatedClassName: 'aos-animate', // class applied on animation
			useClassNames: false, // if true, will add content of `data-aos` as classes on scroll
			disableMutationObserver: false, // disables automatic mutations' detections (advanced)
			debounceDelay: 50, // the delay on debounce used while resizing window (advanced)
			throttleDelay: 99, // the delay on throttle used while scrolling the page (advanced)
			

			// Settings that can be overridden on per-element basis, by `data-aos-*` attributes:
			offset: 120, // offset (in px) from the original trigger point
			delay: 0, // values from 0 to 3000, with step 50ms
			duration: 1200, // values from 0 to 3000, with step 50ms
			easing: 'ease', // default easing for AOS animations
			once: true, // whether animation should happen only once - while scrolling down
			mirror: false, // whether elements should animate out while scrolling past them
			anchorPlacement: 'top-bottom', // defines which position of the element regarding to window should trigger the animation

			});
		jQuery.noConflict(true);
		// window.jQuery = jq;
		jQuery(".all").click(function() {
			console.log("All");
							jQuery([document.documentElement, document.body]).animate({
										  scrollTop: jQuery("#menu-main").offset().top
								  }, 1200);
								  
							jQuery(".all").css("font-weight", "bold");
							jQuery(".design").css("font-weight", "normal");
							jQuery(".film-video").css("font-weight", "normal");
							jQuery(".poetry").css("font-weight", "normal");
							
							jQuery(".one-video").hide();
							jQuery(".one-video").delay(500).slideDown(500);
							jQuery(".two-design").show();
							jQuery(".three-design").show();
							jQuery(".four-design").show();
							jQuery(".five-design").show();
							jQuery(".six-video").show();
							jQuery(".seven-design").show();
							jQuery(".eight-design").show();
							jQuery(".nine-video").show();
							jQuery(".ten-poetry").show();
							jQuery(".eleven-design").show();
						  });
						  
						  //DESIGN
						  jQuery(".design").click(function() {
							console.log("Design");
								  jQuery([document.documentElement, document.body]).animate({
										  scrollTop: jQuery("#menu-main").offset().top
								  }, 1200);
								  
							jQuery(".all").css("font-weight", "normal");
							jQuery(".design").css("font-weight", "bold");
							jQuery(".film-video").css("font-weight", "normal");
							jQuery(".poetry").css("font-weight", "normal");
							jQuery(".installation").css("font-weight", "normal");
							
							// jQuery(".one-video").hide();
							jQuery(".two-design").hide();
							jQuery(".one-video").slideUp(500);
							jQuery(".two-design").slideDown(500);
							jQuery(".three-design").show(); //is also video
							jQuery(".four-design").show();
							jQuery(".five-design").show();
							jQuery(".seven-design").show();
							jQuery(".eight-design").show();
							jQuery(".eleven-design").show();
						  
							jQuery(".six-video").hide();
							jQuery(".nine-video").hide();
							jQuery(".ten-poetry").hide();
						  });
						  
						  //FILM+VIDEO
						  jQuery(".film-video").click(function() {
							console.log("Film");
								  jQuery([document.documentElement, document.body]).animate({
										  scrollTop: jQuery("#menu-main").offset().top
								  }, 1200);
								  
							jQuery(".all").css("font-weight", "normal");
							jQuery(".design").css("font-weight", "normal");
							jQuery(".film-video").css("font-weight", "bold");
							jQuery(".poetry").css("font-weight", "normal");
							
							jQuery(".one-video").hide();
							jQuery(".two-design").slideUp(500);
							jQuery(".one-video").slideDown(500);
							jQuery(".three-design").show(); //is also video
							jQuery(".six-video").show();
							jQuery(".nine-video").show();
						  
							jQuery(".four-design").hide();
							jQuery(".five-design").hide();
							jQuery(".seven-design").hide();
							jQuery(".eight-design").hide();
							jQuery(".ten-poetry").hide();
							jQuery(".eleven-design").hide();
						  });
						  
						  //POETRY
						  jQuery(".poetry").click(function() {
							console.log("Poetry");
							jQuery([document.documentElement, document.body]).animate({
										  scrollTop: jQuery("#menu-main").offset().top
								  }, 1200);
								  
							jQuery(".all").css("font-weight", "normal");
							jQuery(".design").css("font-weight", "normal");
							jQuery(".film-video").css("font-weight", "normal");
							jQuery(".poetry").css("font-weight", "bold");
							
							jQuery(".one-video").hide(); //is also poetry
							jQuery(".one-video").slideDown(500); //is also poetry
							jQuery(".ten-poetry").show();
							
							jQuery(".two-design").hide();
							jQuery(".three-design").hide(); //is also video
							jQuery(".four-design").hide();
							jQuery(".five-design").hide();
							jQuery(".six-video").hide();
							jQuery(".seven-design").hide();
							jQuery(".eight-design").hide();
							jQuery(".nine-video").hide();
							jQuery(".eleven-design").hide();
						  });
						  jQuery(".beforeMyBeginningMoreLink").click(function() {
							jQuery(".onBeforeMyBeginningMoreText").fadeToggle(300);
							if(jQuery('.beforeMyBeginningMoreLink span').text()=="less"){
								  jQuery('.beforeMyBeginningMoreLink').html("<span>more</span> <svg xmlns='http://www.w3.org/2000/svg' width='20' height='20' viewBox='0 0 24 24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round' class='inline feather feather-arrow-right'><line x1='5' y1='12' x2='19' y2='12'></line><polyline points='12 5 19 12 12 19'></polyline></svg>");
							}
							else{
								  jQuery('.beforeMyBeginningMoreLink').html("<svg class='inline w-4' enable-background='new 0 0 71.6 79.4' version='1.1' viewBox='0 0 71.6 79.4' xml:space='preserve' xmlns='http://www.w3.org/2000/svg'> <style type='text/css'> .st0{fill:none; stroke-width:6.5;stroke-miterlimit:10;} </style> <line class='st0' x1='32.9' x2='32.9' y1='75' y2='12.5' stroke='#858585'/> <polyline class='st0' points='9.4 31.9 33 8.3 57.4 32.7' stroke='#858585'/></svg><span>less</span>");
							}
						  });
						  jQuery(".backtotop").click(function() {
							console.log("Clicked on back to top");
							jQuery("html, body").animate({ scrollTop: 0 }, 1500);
							return false;
						  });
						  
	});
	function handleBackToTop(){
							console.log("Clicked on back to top");
							jQuery("html, body").animate({ scrollTop: 0 }, 1500);
							return false;
						  }
</script>

<svelte:head>
	<title>mathew d</title>
	<meta name="description" content="I'm an artist and designer." />
</svelte:head>

<section>
	<video width="1920" height="1080" autoplay="true" muted="true" loop="true" playsinline="true" class="scroll-transition-fade" data-scale="100" style="w-100 transition-duration: initial;">
		<source src="videos/Comp-1_hd-1.mp4">
	</video>
		<br>
		<div style="text-align: center;;" id="menu-main" class="menu-main">
			<br>
			<small><span style="color: #fff;"><a class="all cursor-pointer" rel="history" style="font-weight: bold;">all</a>
				&nbsp; &nbsp; <a class="design cursor-pointer" rel="history" style="font-weight: normal;">design</a> 
				&nbsp; &nbsp; <a class="film-video cursor-pointer" rel="history" style="font-weight: normal;">film+video</a>
				&nbsp; &nbsp; <a class="poetry cursor-pointer" rel="history" style="font-weight: normal;">poetry</a>
				&nbsp; &nbsp;</span></small><br>
			<br>
			<br>
		  </div>
		  <div class="one-video" data-aos="slide-up">
			<div in:fade style="padding:56.25% 0 0 0;position:relative;">
			  <iframe src="https://player.vimeo.com/video/289932054?h=f6cd31e02c&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="before my beginning" class=""></iframe>
			</div>
			<div class="text-content px-2 lg:px-0 max-w-screen-sm">
			  <br>
			  <h2>before my beginning</h2>
			  <div>
				<div>
				  <br>
				  <small>this film is inspired from the idea that everything in creation starts from a thought: the thought, unseen, is the birthplace of that which is seen. with this idea, the story of what life was like before life itself began is mused upon.</small>
				  
				  <small class="onBeforeMyBeginningMoreText" style="display:none;"><br><br>
				  this film is inspired from the idea that everything in creation starts from a thought: the thought, unseen, is the birthplace of that which is seen. with this idea, the story of what life was like before life itself began is mused upon.
				  <br>
				  <br>
				</small>
				  <a class="block cursor-pointer"><span class="link-more beforeMyBeginningMoreLink">more<ArrowRight /></span></a>
				  <br>
				</div>
			  </div>
			  </div>
			  <hr>
		  </div>
		  
	
		  <div class="two-design" data-aos="slide-up">
			<br>
			<Splide aria-label="My Favorite Images" options={ {
				rewind: true,
				rewindSpeed:1,
				autoplay: true,
				interval: 3000,
				speed:1000,
				rewindSpeed:1,
				pagination: false,
			  } }>
				<SplideSlide>
					<img src="images/home/psl-05.png" alt="Image 1"/>
				</SplideSlide>
				<SplideSlide>
					<img src="images/home/psl.jpg" alt="Image 2"/>
				</SplideSlide>
				<SplideSlide>
					<img src="images/home/psl_3.jpg" alt="Image 3"/>
				</SplideSlide>
			  </Splide>
			<div class="text-content px-2 lg:px-0 max-w-screen-sm">
			  <h2><br>
			  portable slit lamp</h2><br>
			  <div>
				<div>
				  <small>
					a handheld slit lamp designed for remote eye screening and off clinic use. this device is used by healthworkers to image the anterior section of the eye.<br>
						<span class="link-more block"><a href="portable-slit-lamp" rel="history"><span class="link-more">more<ArrowRight /></span>
						</small><br>
				</div>
			  </div>
			</div>
			<hr>
		  </div>


		  
		  <div class="three-design three-video" data-aos="slide-up" style="display: block;">
			<br>
			<Image src="images/home/modeling-consionusness.jpg" alt="Modelling Consciousness" />
			<br>
			<br>
			<div class="text-content px-2 lg:px-0 max-w-screen-sm">
			  <h2>modeling consciousness</h2>
			  <div>
				<div>
				  <br>
				  <small>we have been taught that a tree does not move. but in itself, the tree is a hive of activity with visible growth and decay resulting from movement of the elements that make up the tree: radially and vertically extending trunk, flowing tree sap, roots that grow across the forest floor, and so on. thus it moves. &nbsp;</small>
				  <small><a href="modelling-consciousness" class="block" rel="history"><span class="link-more">more<ArrowRight /></span></a></small>
				  <br>
				</div>
			  </div>
			  </div>
			  <hr>
		  </div>

		  <div class="four-design" data-aos="slide-up" style="display: block;">
			<br>
			<Image src="images/home/virtual-showroom.jpg" alt="Virtual Lab" />
			<br>
			<div class="text-content px-2 lg:px-0 max-w-screen-sm">
			  <h2>virtual lab</h2>
				<br>
				<div>
				  <small>in 2021, the pandemic hit and ophthalmology conferences came to a halt. the remidio virtual clinic was concieved as a solution to bring product visibility as a virtual experience to potential customers.</small> 
				  <small><a href="virtual-lab" class="block" rel="history"><span class="link-more">more<ArrowRight /></span></a></small>
				  <br>
				</div>
			  </div>
			  <hr>
		  </div>

		  <div class="five-design" data-aos="slide-up" style="display: block;">
			<br>
			<div style="padding:56.25% 0 0 0;position:relative;">
			  <iframe src="https://player.vimeo.com/video/254954384?h=5a6eadae63" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="video reel" class=""></iframe>
			</div>
			<br>
			<div class="text-content px-2 lg:px-0 max-w-screen-sm">
			  <h2>floor living</h2><br>
			  <div>
				<div>
				  <small>a series of rugs designed to invite the user into different positions of sitting on the floor.</small><br>
				  <div style="display: block;">
					<div class="three" style="display: block;">
					  <a href="floor-living" rel="history">
						<span class="link-more">more<ArrowRight /></span>
					  </a>
					</div>
				  </div><br>
				</div>
			  </div>
			  </div>
			  <hr>
		  </div>

		  <div class="six-video" data-aos="slide-up" style="display: block;">
			<br>
			<div style="padding:56.25% 0 0 0;position:relative;">
			  <iframe src="https://player.vimeo.com/video/782234469?h=cbd129cc36&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="video reel" class=""></iframe>
			</div>
			<div class="text-content px-2 lg:px-0 max-w-screen-sm">
			  <br>
			  <h2>video reel</h2>
			  <br>
			  <small>a reel of my best video work so far.</small><br>
			  <br>
			</div>
			<hr>
		  </div>

		  <div class="seven-design" data-aos="slide-up" style="display: block;">
			<br>
			<Image src="images/home/P1010306.jpg" alt="Storytelling with Patterns" />
			<br>
			<div class="text-content px-2 lg:px-0 max-w-screen-sm">
			  <h2>storytelling with patterns</h2>
			  <br>
			  <div>
				  <small>the story of a lampshade made by a small metalworker in Istanbul is told through a graphic pattern. this pattern reveals the journey of every component across the world before it became a part of the final lamp.</small> 
				  <small>
					<a href="storytelling-with-patterns" class="block" rel="history">
						<span class="link-more">more<ArrowRight /></span></a><br>
				  </div>
			  </div>
			  <hr>
		  </div>

		  <div class="eight-design" data-aos="slide-up" style="display: block;">
			<div style="padding:56.25% 0 0 0;position:relative;">
			  <iframe src="https://player.vimeo.com/video/790747257?h=a564197452" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Remidio Portable Slit Lamp" class=""></iframe>
			</div>
			<br>
			<br>
			<div class="text-content px-2 lg:px-0 max-w-screen-sm">
			  <h2>the ring of trust</h2><br>
				<div>
				  <small>can a design language be applied when the manufacturing process is different for every product a company makes? I created the ring of trust to solve this problem.</small>
					  <a href="ring-of-trust" class="block" rel="history">
						<span class="link-more">more<ArrowRight /></span>
					  </a>
					</div>
				  <br>
			  </div>
			  <hr>
		  </div>
			
			<br>
			
			<div class="nine-video" data-aos="slide-up" style="display: block;">
			  <div style="padding: 56.25% 0px 0px; position: relative;">
				 <iframe src="https://player.vimeo.com/video/786815284?h=f3f26be4a0&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="nanjappa"></iframe>
			  </div>
			  <br>
			  <div class="text-content px-2 lg:px-0 max-w-screen-sm">
				<h2>nanjappa</h2><br>
				<div>
				  <div>
					<small>nanjappa goes about his daily job as a night shift guard. few people know why and how he ended up where he is. this film is an insight into the complex causes behind an ordinary life.</small><br>
					<br>
				  </div>
				</div>
			  </div>
			  <hr>
			</div>

			<div class="ten-poetry" data-aos="slide-up" style="display: block;">
			  <br>
			  <Image src="images/home/DSC00317.jpg" alt="Unapologetic Automatic" />
			  <br>
			  <div class="text-content px-2 lg:px-0 max-w-screen-sm">
				<h2>unapologetic automatic</h2><br>
				<small>my first collection of poetry. illustrated and handbound.</small><br>
				<div class="one" style="display: block;">
				  <div class="three" style="display: block;">
					<div>
					  <div>
						<a href="unapologetic" class="block" rel="history">
							<span class="link-more">more<ArrowRight /></span>
						</a>
					  </div>
					</div>
				  </div>
				</div><br>
			  </div>
			  <hr>
			</div>

			<div class="eleven-design" data-aos="slide-up" style="display: block;">
			  <br>
			  <Image src="images/home/flux.jpg" alt="Flux" />
			  <br>
			  <div class="text-content px-2 lg:px-0 max-w-screen-sm">
				<h2>flux</h2><br>
				<div>
				  <div>
					<small>a culmination of research done on ‘technomagic’ - a word used to describe the blurring boundaries between technology, magic and what seems real. made in collaboration with elsa rambaud and matilde pautelli.
						<br>
						<a href="flux" class="block" rel="history"><span class="link-more">more<ArrowRight /></span></a>
						<br>
					</small>
				  </div>
				</div>			
			  </div>
			  <hr>
			</div>

			<div>
				<br>
				<button class="backtotop" on:click={handleBackToTop}>
<svg class="inline w-4" enable-background="new 0 0 71.6 79.4" version="1.1" viewBox="0 0 71.6 79.4" xml:space="preserve" xmlns="http://www.w3.org/2000/svg">
			   <style type="text/css">
				   .st0{fill:none; stroke-width:6.5;stroke-miterlimit:10;}
			   </style>
			   <line class="st0" x1="32.9" x2="32.9" y1="75" y2="12.5" stroke="#858585"/>
			   <polyline class="st0" points="9.4 31.9 33 8.3 57.4 32.7" stroke="#858585"/>
			   </svg>

			   

					back to top</button><br>
				<br>
				<br>
			  </div>

	<!-- <Counter /> -->
</section>
<!-- 
<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style> -->
