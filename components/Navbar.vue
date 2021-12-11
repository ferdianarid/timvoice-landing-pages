<template>
       <div>
              <div class="font-sans antialiased" id="app">
                     <!-- Class Navbar -->
                     <nav class="navbar flex items-center justify-between flex-wrap  bg-transparent pb-8">
                            <!-- Brand and Logos -->
                            <div class="flex items-center flex-no-shrink mr-6">
                                   <img src="../static/timvoice.svg" alt="timvoicelogo" width="195px">
                            </div>
                     <!-- Hamburger Component -->
                     <div class="block sm:hidden">
                            <button @click="toggle" class="flex items-center px-3 py-2 border rounded text-teal-lighter border-teal-light hover:text-white hover:border-white">
                            <svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/></svg>
                            </button>
                     </div>
                     <!-- Hamburger Action -->
                     <div :class="open ? 'block': 'hidden'" class="w-full flex-grow sm:flex sm:items-center sm:w-auto">
                            <!-- Navigation  Links-->
                            <div class="text-sm font-semibold sm:flex-grow sm:text-right">
                                   <NuxtLink to="/features" class="font-bold no-underline block text-blue-800 mt-4 sm:mx-6 sm:inline-block sm:mt-0 text-teal-lighter hover:text-blue-800 mr-4">
                                          Features
                                   </NuxtLink>
                                   <NuxtLink to="/pricing" class="font-bold no-underline block text-blue-800 mt-4 sm:mx-6 sm:inline-block sm:mt-0 text-teal-lighter hover:text-blue-800 mr-4">
                                          Pricing
                                   </NuxtLink>
                                   <NuxtLink to="/product" class="font-bold no-underline block text-blue-800 mt-4 sm:mx-6 sm:inline-block sm:mt-0 text-teal-lighter hover:text-blue-800 mr-4">
                                          Product
                                   </NuxtLink>
                            </div>
                            <div>

                            <!-- Login Button -->
                            <NuxtLink to="/auth/login" class="font-bold no-underline inline-block border-none text-sm px-4 py-3 mr-3 leading-none bg-white border rounded text-blue-800  hover:border-transparent mt-4 sm:mt-0">Login</NuxtLink>

                            <!-- Get Started Button -->
                            <NuxtLink to="/auth/login" class="px-4 py-2 font-bold no-underline inline-block bg-blue-800 text-white border-none text-sm px-4 py-3 mr-3 leading-none bg-white border rounded text-blue-800  hover:border-transparent mt-4 sm:mt-0">Get Started</NuxtLink>
                            </div>
                     </div>
                     </nav>
              </div>       
       </div>
</template>

<script>
// import Primary Button
import PrimaryButton from "../components/Button/PrimaryButton.vue"
export default {
       name: "Navbar",
       data() {
              return {
                     open: false,
              }
       },
       components: { PrimaryButton },
       methods: {
              toggle() {
                     this.open = !this.open
              }
       }
}
</script>

<style></style>