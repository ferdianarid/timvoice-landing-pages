<template lang="">
       <NuxtLink :to="linkUrl" class="text-center font-bold ml-0 md:ml-1 no-underline inline-block px-4 py-3 leading-none bg-blue-800 border-blue-800 border rounded text-white hover:border-transparent hover:bg-white hover:text-blue-800 mt-4 sm:mt-0">
              <p class="text-lg font-bold">{{ buttonTitle }}</p>
       </NuxtLink>
</template>
<script>
export default {
       name: "PrimaryButton",
       props: ['buttonTitle','linkUrl']
}
</script>
<style lang="">
       
</style>