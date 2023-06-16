<script>
	import Router, {location, link} from 'svelte-spa-router';
  import {home, search, shoppingBag, bullhorn, user} from 'svelte-awesome/icons';
	import Home from './Home.svelte';
	import About from './About.svelte';
	import Cart from './Cart.svelte';
	import Blog from './Blog.svelte';
	import Profile from './Profile.svelte';
	import { AppBar } from '@skeletonlabs/skeleton';
	import { TabGroup, Tab } from '@skeletonlabs/skeleton';
	import Icon from 'svelte-awesome';


	import '@skeletonlabs/skeleton/themes/theme-skeleton.css';
// This contains the bulk of Skeletons required styles:
// NOTE: this will be renamed skeleton.css in the v2.x release.
import '@skeletonlabs/skeleton/styles/skeleton.css';

// Finally, your application's global stylesheet (sometimes labeled 'app.css')
import './app.postcss';
</script>

<AppBar gridColumns="grid-cols-3" slotDefault="place-self-center" slotTrail="place-content-end" class="sticky top-0 bg-white z-10">
	<svelte:fragment slot="lead">=</svelte:fragment>
	FASHOP
</AppBar>

<Router routes={{
	'/': Home,
	'/item': About,
	'/cart': Cart,
	'/social': Blog,
	'/profile': Profile,
}} />


<TabGroup 
	justify="justify-center"
	active="variant-filled-primary"
	hover="hover:variant-soft-primary"
	flex="flex-1 lg:flex-none"
	rounded=""
	border=""
	class="bg-surface-100-800-token w-full sticky bottom-0 bg-white"
>

	<Tab name="books" value={0}>
		<a href="/">
			<Icon data="{home}" />
		</a>
	</Tab>
	<Tab name="books" value={0}>
		<a href="/#/item">
			<Icon data="{search}" />
		</a>
	</Tab>
	<Tab name="books" value={0}>
		<a href="/#/cart">
			<Icon data="{shoppingBag}" />
		</a>
	</Tab>
	<Tab name="books" value={0}>
		<a href="/#/social">
			<Icon data="{bullhorn}" />
		</a>
	</Tab>
	<Tab name="books" value={0}>
		<a href="/#/profile">
			<Icon data="{user}" />
		</a>
	</Tab>
</TabGroup>