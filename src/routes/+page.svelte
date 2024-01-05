<script>

import Carousel from '$lib/components/Carousel.svelte';
import { Accordion, AccordionItem } from '@skeletonlabs/skeleton';
import Icon from '@iconify/svelte';
</script>



<div class="card p-4 max-w-6xl mx-auto m-4">
	<div class="h3 text-4xl text-center p-4 font-bold">Welcome to Inamandla Contractors</div>
	<p class="text-lg">We are a full service Construction Company dedicated to building and improving residential and commercial structures according to client needs and desires. 
		Founded in 2020 and based in Shakaskraal, our team is ready to give your space whatever updates it requires. 
		Just give us a call or write us a note and we’ll get back to you with a quote.</p>
	<p class="text-2xl text-center p-4">You dream it. We build it.</p>	
	
	</div>

	<div class="card p-4 max-w-6xl mx-auto m-4">
		<div class="h3 text-4xl text-center p-4 font-bold">Our Services</div>
		<Accordion>
			<AccordionItem>
				<svelte:fragment slot="lead"><Icon icon="fa6-solid:helmet-safety" width="2em"  /></svelte:fragment>
				<svelte:fragment slot="summary"><div class="text-2xl">Construction</div></svelte:fragment>
				<svelte:fragment slot="content"><p class="text-lg">We specialize in residential homes but have the expertise to handle almost any requirement big or small.</p></svelte:fragment>
			</AccordionItem>
			<AccordionItem>
				<svelte:fragment slot="lead"><Icon icon="mdi:tools" width="2em" /></svelte:fragment>
				<svelte:fragment slot="summary"><div class="text-2xl">Repair</div></svelte:fragment>
				<svelte:fragment slot="content"><p class="text-lg">Our team will attend to any repair work, renovation or maintenance you may require. We're open to having a look at what you need to offer our advice.</p></svelte:fragment>
			</AccordionItem>
			<AccordionItem>
				<svelte:fragment slot="lead"><Icon icon="tabler:tools" width="2em" /></svelte:fragment>
				<svelte:fragment slot="summary"><div class="text-2xl">Design</div></svelte:fragment>
				<svelte:fragment slot="content"><p class="text-lg">The best projects start with a special yet practical design. We can help you get your vision onto paper before any soil is broken.</p></svelte:fragment>
			</AccordionItem>
			<AccordionItem>
				<svelte:fragment slot="lead"><Icon icon="fluent-mdl2:company-directory" width="2em" /></svelte:fragment>
				<svelte:fragment slot="summary"><div class="text-2xl">Company Profile</div></svelte:fragment>
				<svelte:fragment slot="content"><p class="text-lg">Inamandla Contractors is a privately owned business based on the North Coast of KZN. We started from humble beginnings in 2001 but have grown into a fully fledged building solution. Using our almost 20 years of experience we decided to start our own building business in 2020 and Inamandla Contractors was born. Forming our own end to end solution allows us to control a project from start to finish which comes with many advantages... We can ensure our workmanship, maintain our excellent reputation and work exclusively with our most trusted partners. We have worked in most estates on the North Coast and are registered with the NHBRC.</p>
				<br>
				<p class="text-lg">What are you needing help with? Contact us to take us through your needs.</p></svelte:fragment>
			</AccordionItem>
			<!-- ... -->
		</Accordion>
		<div class="logo-cloud grid-cols-1 lg:!grid-cols-3 gap-0.5 max-w-6xl mx-auto m-4">
		
			<a class="logo-item"  href="https://www.simbithi.com/"><img src="/simbithi-logo.png" alt=""></a>
			<a class="logo-item"  href="https://www.nhbrc.org.za/"><img src="/NHBRC.png" class="logo-item" alt=""></a>
			<a class="logo-item"  href="https://palmlakesfamilyestate.co.za/"><img src="/palmlakes-logo.png" class="logo-item" alt=""></a>
			
		</div>
		</div>

		

<div class="card p-4 max-w-6xl mx-auto">
	<header class="card-header text-4xl text-center font-bold">Recent Projects</header>
	<div class="p-4">
<Carousel />
</div>
</div>




<div class="card p-2 max-w-6xl mx-auto m-4">
	
	<div class="h3 text-4xl text-center p-4 font-bold">Contact Us</div>
	<div class="text-xl text-center font-semibold">Call: 0727478170</div>
	<div class="text-xl text-center font-semibold">Email: inamandlacontractors@gmail.com</div>
	<div class="p-4 text-lg text-center">482 Salt Rock Rd Dolphin Coast, South Africa</div>
</div>
