<script>
	import { Carousel } from 'flowbite-svelte';
	import CarouselCard from './CarouselCard.svelte';
	import 'flowbite';

	const images = [
		{
      alt: 'Cosmic timetraveler',
      src: 'https://templesofindia.org/assets/compressed/de57bb046af9aedd4f39566099997f21_942.png',
      title: 'temple image'
    },
    {
      alt: 'Cristina Gottardi',
      src: 'https://templesofindia.org/assets/compressed/1c9d49ab0497a1ac22bb73c2c681e3e6_942.png',
      title: 'cristina-gottardi-CSpjU6hYo_0-unsplash.com'
    },
    {
      alt: 'Johannes Plenio',
      src: 'https://templesofindia.org/assets/compressed/tofi-banner.jpg',
      title: 'johannes-plenio-RwHv7LgeC7s-unsplash.com'
    },
	]
	
	let visited = false;
	let favorite = false;
	let section1 = true;
	let section2 = true;
	let section3 = true;
	let section4 = false;
	let section5 = true;
	let section6 = true;
	let section7 = false;
	let section8 = false;
	let section9 = false;
	let section10 = false;
	let section11 = false;
	function showContent1() {
		section1 = !section1
	}
	function showContent2() {
		section2 = !section2
	}
	function showContent3() {
		section3 = !section3
	}
	function showContent4() {
		section4 = !section4
	}
	function showContent5() {
		section5 = !section5
	}
	function showContent6() {
		section6 = !section6
	}
	function showContent7() {
		section7 = !section7
	}
	function showContent8() {
		section8 = !section8
	}
	function showContent9() {
		section9 = !section9
	}
	function showContent10() {
		section10 = !section10
	}
	function showContent11() {
		section11 = !section11
	}
	function changeVisited() {
		visited = !visited
	}
	function changeFavorite() {
		favorite = !favorite
	}
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Temple of india" />
	</svelte:head>

<section>
    
	
	<div class="main-container">
			<div class="max-w-4xl space-y-4" id="carousel-card">
				<Carousel {images} imgClass="object-contain h-full w-fit rounded-sm carousel-image" duration="3000" id="carousel" class="rounded-md border-4 border-white dark:border-gray-800 min-h-[320px] bg-gray-200" />
			</div>
		<div class="main-container-2">
			<div class="content-card">
				<h1 class="main-head">Sri Ranganathar Temple</h1>
				<p class="main-para">Vishnu</p>
				<br />
				<div class="section-details-card">
					<button type="button" on:click={showContent1} class={section1 ? "section" : "section section-close"}>
						{#if section1}
							<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-up"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 15l6 -6l6 6" /></svg>
						{:else}
							<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-down"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 9l6 6l6 -6" /></svg>
						{/if}
						<p class="section-name">Special Features</p>
					</button>
					<a href="https://templesofindia.org/login">
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
					</a>
				</div>
					{#if section1}
						<div class="section-content">
							<p class="bold-text">Foundation Year</p>
							<p class="text">500-1000 years old</p>
							<br />
							<p class="bold-text">Sthala Tree</p>
							<br />
							<p class="bold-text">Theertham</p>
							<p class="text">Palsunai, Padma theertham, Sengothai Sunai, Kannimar Sunai, Pasumani Sunai</p>
							<br />
							<p class="bold-text">Ratham</p>
							<br />
							<p class="bold-text">Architecture</p>
							<p class="text">Dravidian Architecture</p>
							<br />
							<p class="bold-text">Other Speciality</p>
							<p class="text">All merciful Lord Ranganatha appears in a standing form facing east pleasing the mind of His devotees.</p>
							<br />
							<hr />
						</div>
					{/if}
				
			
			<div class="section-details-card">
				<button type="button" on:click={showContent2} class={section2 ? "section" : "section section-close"}>
					{#if section2}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-up"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 15l6 -6l6 6" /></svg>
					{:else}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-down"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 9l6 6l6 -6" /></svg>
					{/if}
					<p class="section-name">Sthala Puran</p>
				</button>
				<a href="https://templesofindia.org/login">
					<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
				</a>
			</div>
				{#if section2}
					<div class="section-content">
						
						<p class="text">Maharshi Kalava was in penance for a quite number of years to have the darshan of Lord Narayana.  One Durmadhan, son of a Gandarva Viswasu by name was bathing in the tank with his wives.  Maharshi Vasishta was returning from Mount Kailash after a darshan of Lord Shiva.  Seeing the sage, Durmadha’s wives stopped bathing and came out of the tank in respect to the sage.  But Durmadha continued bathing nude.  Angry Vasishta cursed Dhurmada to be born a demon.  The wives fell at the feet of Sage Vasishta and begged for relief.  Responding to their prayer, sage said that their husband would be back to them in a short time.</p>
						<br />
						<br />
						<br />
						<br />
						<p class="text">Durmadha wandering here and there as a demon saw Maharshi Kalava and began to harass him.  Rishi prayed to Lord Narayana for protection.  Lord granted darshan to Rishi and controlled the demon.  With the touch of Lord, Durmadha was relieved of his curse.  It is believed that this event took place here.</p>
						<br />
						<br />
						<br />
						<br />
						<p class="text">The other story is that a king Nanda Boopala, ruling this region renounced his kingdom and set out for penance on Lord Narayana.  His son Darma Gupta became the king and was ruling the region righteously.  When he was in the forest for hunting, dusk set in and the king could not find the way to the camp.  He climbed on a tree and began chanting the Gayatri Mantra.  A bear, chased by a lion also came to the tree branch and sat along with the king.</p>
						<br />
						<br />
						<br />
						<br />
						<p class="text">The king said to the bear that both would be at a risk if they returned to the ground.  The bear suggested that the king may sleep half the night when it would take care of him and that it would sleep the remaining night protected by the king.  While the king was sleeping the lion under the tree asked the bear to push the king down.  The bear simply said that it could not commit a sin as breach of trust.  When the kin woke up and the bear started sleeping the lion made the suggestion to the king.  Thoughtlessly, the king obliged the lion pushing the bear down.  Shocked by the behaviour of the king, the bear luckily escaping the attack of the lion, cursed the king to become a lunatic.  King Nanda Boopala seeing the condition of son Darma Gupta, took him to Sage Jaimini for the cure.  Sage suggested that he should have a dip in Palamalai Theertha and worship Lord Ranganatha for recovery.  Darma Gupta was thus saved by Palamalai Lord Ranganatha.</p>
						
						<br />
						<hr />
					</div>
				{/if}
			<div class="section-details-card">
				<button type="button" on:click={showContent3} class={section3 ? "section" : "section section-close"}>
					{#if section3}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-up"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 15l6 -6l6 6" /></svg>
					{:else}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-down"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 9l6 6l6 -6" /></svg>
					{/if}
					<p class="section-name">Architecture</p>
				</button>
				<a href="https://templesofindia.org/login">
					<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
				</a>
			</div>
				{#if section3}
					<div class="section-content">
						
						<p class="text">All merciful Lord Ranganatha appears in a standing form facing east pleasing the mind of His devotees.  Thumbikkai Azhwar and Mother grace the devotees from their respective shrines.  Adequate space is created around the temple to facilitate car festival and movement of devotees during festival times.  Many visit the temple frequently as the environment and the climate are helpful to keep them healthy and free from any disease.  Irulars, a tribal community are living near the temple.  The car of the temple is aesthetically made by skilled craftsmen.</p>
						<br />
						<br />
						<br />
						<br />
						<p class="text">The devotee crowd is huge on new moon days and Saturdays.  There are shrines for Lord Vinayaka, Sri Anjaneya and Acharya Sri Ramanuja.</p>
						<br />
						
						<br />
						<hr />
					</div>
				{/if}
			<div class="section-details-card">
				<button type="button" on:click={showContent4} class={section4 ? "section" : "section section-close"}>
					{#if section4}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-up"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 15l6 -6l6 6" /></svg>
					{:else}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-down"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 9l6 6l6 -6" /></svg>
					{/if}
					<p class="section-name">Alankar of Deity</p>
				</button>
				<a href="https://templesofindia.org/login">
					<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
				</a>
			</div>
				{#if section4}
					<div class="section-content">
						<br />
						<br />
						<hr />
					</div>
				{/if}

			<div class="section-details-card">
				<button type="button" on:click={showContent5} class={section5 ? "section" : "section section-close"}>
					{#if section5}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-up"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 15l6 -6l6 6" /></svg>
					{:else}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-down"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 9l6 6l6 -6" /></svg>
					{/if}
					<p class="section-name">Prayers and Benefits</p>
				</button>
				<a href="https://templesofindia.org/login">
					<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
				</a>
			</div>

				{#if section5}
					<div class="section-content">
						<br />
						<p class="bold-text">Special Vratas and Prayers</p>
						<p class="text">Those facing the impact of some curses pray for relief.</p>
						<br />
						<br />
						<p class="bold-text">Offerings to Deity</p>
						<p class="text">Devotees perform Tirumanjanam to Lord and Mother with sweet pudding-sarkarai pongal nivedhana.</p>
						<br />
						<p class="bold-text">Stotras and Mantras</p>
						<br />
						<br />
						<hr />
					</div>
				{/if}

			<div class="section-details-card">
				<button type="button" on:click={showContent6} class={section6 ? "section" : "section section-close"}>
					{#if section6}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-up"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 15l6 -6l6 6" /></svg>
					{:else}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-down"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 9l6 6l6 -6" /></svg>
					{/if}
					<p class="section-name">Festivals</p>
				</button>
				<a href="https://templesofindia.org/login">
					<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
				</a>
			</div>
				{#if section6}
					<div class="section-content">
						<br />
						<p class="text">Car festival is celebrated in the temple on Chitra Poornima day in April-May.</p>
						<br />
						<br />
						<hr />
					</div>
				{/if}
			<div class="section-details-card">
				<button type="button" on:click={showContent7} class={section7 ? "section" : "section section-close"}>
					{#if section7}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-up"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 15l6 -6l6 6" /></svg>
					{:else}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-down"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 9l6 6l6 -6" /></svg>
					{/if}
					<p class="section-name">Sodasha Upcharas</p>
				</button>
				<a href="https://templesofindia.org/login">
					<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
				</a>
			</div>

				{#if section7}
					<div class="section-content">
						<br />
						<hr />
					</div>
				{/if}
			<div class="section-details-card">
				<button type="button" on:click={showContent8} class={section8 ? "section" : "section section-close"}>
					{#if section8}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-up"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 15l6 -6l6 6" /></svg>
					{:else}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-down"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 9l6 6l6 -6" /></svg>
					{/if}
					<p class="section-name">Prasadhas</p>
				</button>
				<a href="https://templesofindia.org/login">
					<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
				</a>
			</div>
		
				{#if section8}
					<div class="section-content">
						<br />
						<hr />
					</div>
				{/if}

			<div class="section-details-card">			
				<button type="button" on:click={showContent9} class={section9 ? "section" : "section section-close"}>
					{#if section9}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-up"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 15l6 -6l6 6" /></svg>
					{:else}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-down"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 9l6 6l6 -6" /></svg>
					{/if}
					<p class="section-name">Social Activities</p>
				</button>
				<a href="https://templesofindia.org/login">
					<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
				</a>
			</div>
				{#if section9}
					<div class="section-content">
						<br />
						<p class="bold-text">Annadhan</p>
						<br />
						<p class="bold-text">Marriage</p>
						<br />
						<p class="bold-text">Ear Boring</p>
						<br />
						<p class="bold-text">Head Shave</p>
						<br />
						<p class="bold-text">Danaas</p>
						<br />
						<p class="bold-text">Education Facilities</p>
						<br />
						<p class="bold-text">Social Drives</p>
						<br />
						<p class="bold-text">Other Activities</p>
						<br />
						
						<hr />
					</div>
				{/if}

			<div class="section-details-card">
				<button type="button" on:click={showContent10} class={section10 ? "section" : "section section-close"}>
					{#if section10}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-up"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 15l6 -6l6 6" /></svg>
					{:else}
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-chevron-down"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 9l6 6l6 -6" /></svg>
					{/if}
					<p class="section-name">Arjita Seva</p>
				</button>
				<a href="https://templesofindia.org/login">
					<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
				</a>
			</div>
				{#if section10}
					<div class="section-content">
						<br />
						<hr />
					</div>
				{/if}
				<div class="section-details-card">
					<button type="button" on:click={showContent11} class={section11 ? "section" : "section section-close"}>
						<p class="section-name detail">Tags</p>
					</button>
					<a href="https://templesofindia.org/login">
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
					</a>
				</div>
					
					{#if section11}
						<div class="section-content">
							<br />
							<hr />
							<br/>
							<div class="btn-card">
								<button class="submit-change">Submit Changes</button>
							</div>
							
						</div>
					{/if}
				<p class="section-name detail contri">Contributors</p>
				<hr />
				<br />
				<p class="section-name detail">Comments</p>
				<br />

			</div>
			<div class="side-bar">
				<div class="visit-fav-card">
					<button type="button" on:click={changeVisited} class="visited-btn">
						{#if visited}
							<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQkZBCRv1yG6_F7P2NPEpwV7C_6gYYnt02OcWOYXiqBNA&s" alt="namaste" class="visited" />
							
						{:else}
							<img src="https://cdn-icons-png.flaticon.com/512/317/317833.png" alt="namaste" class="visited" />
						{/if}
						Visited
					</button>

					<button type="button" on:click={changeFavorite} class="visited-btn">
						
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class={favorite ? "icon icon-tabler icons-tabler-outline icon-tabler-heart visited fav" : "icon icon-tabler icons-tabler-outline icon-tabler-heart visited"}><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M19.5 12.572l-7.5 7.428l-7.5 -7.428a5 5 0 1 1 7.5 -6.566a5 5 0 1 1 7.5 6.572" /></svg>
						Favorite
					</button>
				</div>

				<div class="details-card">
					<div class="section-details-card">
						<p class="section-name detail">Location</p>
						<button type="button" class="visited-btn">
							<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
						</button>
					</div>
					<a href="https://www.google.com/maps/dir//10.9513265,77.0145986/@10.9513265,77.0145986,18z?entry=ttu" target="_blank" class="google-map">View on Maps</a>
					<p class="google-map location">Unnamed Road, Anbu Nagar, Podanur, Coimbatore, Tamil Nadu 641023

					</p>
					<iframe title="icon" width="100%" height="150" src="https://www.openstreetmap.org/export/embed.html?bbox=76.98841094970705%2C10.94371989773879%2C77.02857971191408%2C10.970685000386721&amp;layer=mapnik&amp;marker=10.957202756183145%2C77.00849533081055" style="border: 1px solid black"></iframe>
					<br />
					<br />
					<div class="section-details-card">
						<p class="section-name detail">Open Timings</p>
						<button type="button" class="visited-btn">
							<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
						</button>
					</div>
					<p class="timing-text">Alldays: 07:00 am - 09:00 am
						<br />
						<br />
					Alldays: 07:00 am - 09:00 am
					</p>
					<br />
					
					<div class="section-details-card">
						<p class="section-name detail">Pooja Timings</p>
						<button type="button" class="visited-btn">
							<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
						</button>
					</div>
					<br />
				
					<div class="section-details-card">
						<p class="section-name detail">Other Deities</p>
						<button type="button" class="visited-btn">
							<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
						</button>
					</div>
					<br />
				
					<div class="section-details-card">
						<p class="section-name detail ameni">Amenities</p>
						<button type="button" class="visited-btn">
							<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
						</button>
					</div>
					<br />
					<div class="amenities-points">
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#119400"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-check"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M5 12l5 5l10 -10" /></svg>
						<p class="amenities-name">Drinking Water</p>
					</div>
					<div class="amenities-points">
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#119400"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-check"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M5 12l5 5l10 -10" /></svg>
						<p class="amenities-name">Pooja Item Shops</p>
					</div>
					<div class="amenities-points">
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#119400"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-check"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M5 12l5 5l10 -10" /></svg>
						<p class="amenities-name">Restaurants Nearby</p>
					</div>
					<div class="amenities-points">
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#119400"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-check"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M5 12l5 5l10 -10" /></svg>
						<p class="amenities-name">Restroom</p>
					</div>
					<br />

					<div class="section-details-card">
						<p class="section-name detail">How to reach?</p>
						<button type="button" class="visited-btn">
							<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
						</button>
					</div>
					<div class="section-details-card reaching">
						<p class="bold-text">Nearest Bus Station</p>
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#f10909"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-bus logo"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 17m-2 0a2 2 0 1 0 4 0a2 2 0 1 0 -4 0" /><path d="M18 17m-2 0a2 2 0 1 0 4 0a2 2 0 1 0 -4 0" /><path d="M4 17h-2v-11a1 1 0 0 1 1 -1h14a5 7 0 0 1 5 7v5h-2m-4 0h-8" /><path d="M16 5l1.5 7l4.5 0" /><path d="M2 10l15 0" /><path d="M7 5l0 5" /><path d="M12 5l0 5" /></svg>
					</div>
					<p class="text">Gandhipuram</p>

					<div class="section-details-card reaching">
						<p class="bold-text">Nearest Railway Station</p>
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#f10909"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-train"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M21 13c0 -3.87 -3.37 -7 -10 -7h-8" /><path d="M3 15h16a2 2 0 0 0 2 -2" /><path d="M3 6v5h17.5" /><path d="M3 10l0 4" /><path d="M8 11l0 -5" /><path d="M13 11l0 -4.5" /><path d="M3 19l18 0" /></svg>
					</div>
					<p class="text ">Coimbatore</p>
					
					<div class="section-details-card reaching">
						<p class="bold-text">Nearest Airport</p>
						<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#f10909"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-plane"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M16 10h4a2 2 0 0 1 0 4h-4l-4 7h-3l2 -7h-4l-2 2h-3l2 -4l-2 -4h3l2 2h4l-2 -7h3z" /></svg>
					</div>
					<p class="text ">Coimbatore</p>
					<br />
					<br />
					<div class="section-details-card">
						<p class="section-name detail">Contact Details</p>
						<button type="button" class="visited-btn">
							<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="#000000"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-pencil"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 20h4l10.5 -10.5a2.828 2.828 0 1 0 -4 -4l-10.5 10.5v4" /><path d="M13.5 6.5l4 4" /></svg>
						</button>
					</div>
					<p class="text reaching">Name</p>
					<p class="text reaching">Phone <br />
						+91-94433 48564</p>
					<p class="text reaching">Name</p>
					<p class="text reaching">Phone <br />
						+91-94433 48564</p>
					<p class="text reaching">Website</p>
				</div>
			</div>
		</div>
		<div class="feedback-card">
			<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-message-report feedback-logo"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M18 4a3 3 0 0 1 3 3v8a3 3 0 0 1 -3 3h-5l-5 3v-3h-2a3 3 0 0 1 -3 -3v-8a3 3 0 0 1 3 -3h12z" /><path d="M12 8v3" /><path d="M12 14v.01" /></svg>
		</div>
	</div>
</section>

