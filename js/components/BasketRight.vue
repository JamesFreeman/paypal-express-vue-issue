<template>
	<div>
		<div id="checkout">
			<div data-sticky data-anchor="checkout" data-margin-top="0" data-sticky-on="large">
				<PayPal amount="10.00" currency="GBP" :client="paypal" env="sandbox"></PayPal>
			</div>
		</div>
	</div>
</template>
<script>
	import PayPal from 'vue-paypal-checkout'

	export default{
		data() {
		    return {
		      paypal: {
		        sandbox: 'AZDh28XUkdZSgT7CaR79z4u6cm-P2SJdIYyPjugeT5gbD5n2gS5h-JiQG0dpT5_elt0fDrZ6QvIt67ET',
		        production: ''
		      }
		    }
		  },
		  components: {
		    PayPal
		  }
	}
</script>
