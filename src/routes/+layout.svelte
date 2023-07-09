<script lang='ts'>
	// The ordering of these imports is critical to your app working properly
	import '@skeletonlabs/skeleton/themes/theme-crimson.css';
	// If you have source.organizeImports set to true in VSCode, then it will auto change this ordering
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	// Most of your app wide CSS should be put in this file
	import '../app.postcss';
	import { AppShell, AppBar, LightSwitch } from '@skeletonlabs/skeleton';
	import Footer from '$lib/components/Footer.svelte';
	import Icon from '@iconify/svelte';
</script>


<AppShell>
	<svelte:fragment slot="header">
		
		
<AppBar gridColumns="grid-cols-1" slotDefault="place-self-center" slotTrail="place-content-end">
	<svelte:fragment slot="lead"> </svelte:fragment>
	<img src="/logo.png" alt="" class="w-72 col-span-1">
	<svelte:fragment slot="trail"> </svelte:fragment>
</AppBar>

<div class="grid grid-cols-1 sm:grid-cols-3 justify-items-center max-w-4xl mx-auto">
	<div class="flex col-span-1 items-center font-bold ">Contact Us: </div>
	<div class="flex col-span-1 items-center font-bold "><Icon class="mx-1" icon="ph:phone-fill"/>0727478170</div>
	<div class="flex col-span-1 items-center font-bold "><Icon class="mx-1" icon="iconamoon:email-bold" />inamandlacontractors@gmail.com</div>
</div>

	</svelte:fragment>
	<!-- (sidebarLeft) -->
	<!-- (sidebarRight) -->
	<!-- (pageHeader) -->
	<!-- Router Slot -->
	<slot />
	<!-- ---- / ---- -->
	<svelte:fragment slot="pageFooter"><Footer /></svelte:fragment>
	<!-- (footer) -->
</AppShell>


