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
		
		
<AppBar gridColumns="grid-cols-3" slotDefault="place-self-center" slotTrail="place-content-end">
	<svelte:fragment slot="lead"><img src="/logo.png" alt="" class="w-72"></svelte:fragment>
	
	<svelte:fragment slot="trail">
	
	
	<div class="grid grid-rows-2 grid-flow-col gap-4">
	
	<div class="flex items-center"><Icon class="mx-1" icon="ph:phone-fill"/>0727478170</div>
	<div class="flex items-center"><Icon class="mx-1" icon="iconamoon:email-bold" />mandla@inamandlacontractors.co.za</div>
	</div></svelte:fragment>
</AppBar>


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


