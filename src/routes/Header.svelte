<script>
	import { page } from '$app/stores';
	import "./home.css"
</script>

<header>
	<div class="nav-bar-sm">
		<div>
			<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="1.25"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-menu-2 menu"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 6l16 0" /><path d="M4 12l16 0" /><path d="M4 18l16 0" /></svg>
		</div>
		<a href="https://templesofindia.org/" class="brand-logo black-text">
			<img src="https://templesofindia.org/assets/images/tofi_logo/tofi-logo_navbar.png" alt="SvelteKit" class="logo"/>
			Temples of India
		</a>
		<a href="https://templesofindia.org/">
			<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="1.25"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-search menu"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M10 10m-7 0a7 7 0 1 0 14 0a7 7 0 1 0 -14 0" /><path d="M21 21l-6 -6" /></svg>
		</a>
	</div>

	<div class="nav-bar">
		<a href="/" class="brand-logo black-text">
			<img src="https://templesofindia.org/assets/images/tofi_logo/tofi-logo_navbar.png" alt="SvelteKit" class="logo"/>
			Temples of India
		</a>
		<div class="menu-card">
			<svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="none"  stroke="currentColor"  stroke-width="2"  stroke-linecap="round"  stroke-linejoin="round"  class="icon icon-tabler icons-tabler-outline icon-tabler-menu-2 menu-logo"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M4 6l16 0" /><path d="M4 12l16 0" /><path d="M4 18l16 0" /></svg>
		</div>
		<ul class="nav-list">
			<li class="nav-item" >
				<a href="https://templesofindia.org/">Home</a>
			</li>
			<li class="nav-item" >
				<a href="https://templesofindia.org/">Search</a>
			</li>
			<li class="nav-item" >
				<a href="https://templesofindia.org/nearbyTemples">Nearby Temple</a>
			</li>

			<li class="nav-item" >
				<a href="https://templesofindia.org/addTempe">
				
					Add Temples</a>
			</li>
			

			<li class="nav-item" >
				<a href="https://templesofindia.org/aboutUs">About Us</a>
			</li>

			<li class="nav-item" >
				<a href="https://templesofindia.org/login">Login</a>
			</li>
		</ul>
	</div>
</header>
