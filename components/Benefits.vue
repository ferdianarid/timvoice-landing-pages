<template lang="">
<div class="flex flex-col">
       <div v-for="list in benefits">
       <div class="w-full flex py-6 px-8 bg-[#F7F8FD] rounded-xl my-2">
		<!-- images -->
              <div class="w-1/4">
                     <img class="scale-75" :src="list.url" alt="currency" width="100%" />
              </div>
		<!-- description -->
              <div class="w-3/4 ml-2">
                     <h1 class="text-heading-md fontBold">{{ list.title }}</h1>
                     <p class="text-lg-regular text-gray-500">{{ list.subtitle }}</p>
              </div>
       </div>
       </div>
</div>
</template>
<script>
export default {
       data() {
              return {
                     benefits: [
				{
					id: 1,
					url: "https://res.cloudinary.com/luminous/image/upload/v1638523240/currency_dqt1a0.svg",
					title: "Get Paid Faster",
					subtitle: "Create and customize invoices, receive updates about payment."
				},
				{
					id: 2,
					url: "https://res.cloudinary.com/luminous/image/upload/v1638523240/briefcase_cc1txv.svg",
					title: "Win More Work",
					subtitle: "Create and customize invoices, receive updates about payment."
				},
				{
					id: 3,
					url: "https://res.cloudinary.com/luminous/image/upload/v1638523240/shield_opluej.svg",
					title: "Protect Business",
					subtitle: "Create and customize invoices, receive updates about payment."
				}
			]
              }
       }
}
</script>
<style lang="">
       
</style>