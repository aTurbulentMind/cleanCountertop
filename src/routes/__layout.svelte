<script>
	import Nav from '$lib/Nav.svelte';
</script>


<div class="body">
 <!-- <div class="logo"><img src="/src/assets/img/LogoTransparentDark.png" alt=""></div>-->

	<Nav />

	<slot />

	
</div>

<style lang="scss">
	@import 'vari';
	@import 'components';

	

	* {
		margin: -8px;
		
	}

	

	.logo {
		overflow-y:hidden;
		margin-top: 5px;

		img {
		width: 80%;
		height: 80%;
		
	}
	}

	
	
		
</style>